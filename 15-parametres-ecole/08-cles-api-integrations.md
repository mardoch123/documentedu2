---
id: 15-08-cles-api-integrations
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-08-cles-api-integrations
emoji: "🔑"
titre: "Clés API & intégrations tierces"
resume: "Cette page branche votre école sur des services externes : reCAPTCHA (protection anti-robots des formulaires publics d'inscription), numéro/token WhatsApp (envoi via votre propre compte WhatsApp Bu..."
audiences: [school_admin]
---
# 🔑 Clés API & intégrations tierces

## 🎯 Rôle
Cette page branche votre école sur des **services externes** : **reCAPTCHA** (protection
anti-robots des formulaires publics d'inscription), **numéro/token WhatsApp** (envoi via
votre propre compte WhatsApp Business), et autres **clés d'intégration** selon votre
abonnement. Une clé correctement saisie = le service externe **fonctionne pour votre école**
; une clé erronée = l'erreur silencieuse côté destinataire.

## ✅ Prérequis
1. Être **School Admin** avec la permission « school-setting-manage » et la fonction
   **Website Management** à l'abonnement.
2. Avoir **récupéré la clé auprès du service externe** :
   - reCAPTCHA : sur `google.com/recaptcha` → créer un site → copier **Site key** et
     **Secret key** ;
   - WhatsApp : **Phone number ID** et **Access token** de votre compte WhatsApp Business
     (sinon utiliser le WhatsApp partagé EduEasy — voir *11*).
3. Accès : **Paramètres → Third-party APIs** (`school-settings.third-party`).

## 🟢 Saisir une clé (étape par étape)
1. Ouvrez **Third-party APIs**.
2. Collez la valeur dans le **champ de la clé voulue** (`SCHOOL_RECAPTCHA_SITE_KEY`,
   `SCHOOL_RECAPTCHA_SECRET_KEY`, `whatsapp_phone_number_id`, `whatsapp_access_token`…).
3. **Enregistrez** (`school-settings.third-party.update`).
4. **Testez immédiatement** :
   - reCAPTCHA : ouvrez le **formulaire public d'inscription** et vérifiez que le défi
     apparaît ;
   - WhatsApp : bouton **test** dédié (`school-settings.third-party.test-whatsapp`) →
     un message de test doit partir.

## ✏️ Modifier / remplacer une clé
1. Revenez sur la page, **collez la nouvelle clé** par-dessus l'ancienne, enregistrez,
   re-testez.
2. Après une **révocation** chez le fournisseur (clé compromise), **remplacez-la vite** :
   l'ancienne clé continuait à être utilisée jusqu'ici.

## 🔴 Supprimer / ♻️ Restaurer
- ⚠️ **Effacer une clé = désactiver l'intégration** (ex. plus de reCAPTCHA sur
  l'inscription). **Notez l'ancienne valeur** avant effacement : la « restauration » est une
  simple **re-saisie**.
- Les clés ne s'exportent pas ; le Support EduEasy peut vérifier qu'une clé est **bien
  enregistrée** (jamais le contraire : ne communiquez **jamais** vos secrets par email/social).

## ⚠️ Bon à savoir
- **Copier-coller, jamais retaper** : les clés sont de longues suites ; une lettre manquée =
  échec mystérieux.
- **Pas d'espaces** au début/à la fin lors du collage.
- **reCAPTCHA = protection des inscriptions en ligne** : fortement recommandé si votre
  formulaire public est ouvert.
- La **validation EMECEP** (intégration ministère) se teste depuis un autre bouton
  (`school-settings.test-emecef`).
- Les paiements en ligne (FeexPay/MoMo) se règlent dans *03-moyens-de-paiement-ecole.md*,
  pas ici.
