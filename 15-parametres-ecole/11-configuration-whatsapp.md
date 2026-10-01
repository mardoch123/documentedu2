---
id: 15-11-configuration-whatsapp
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-11-configuration-whatsapp
emoji: "💬"
titre: "Configuration WhatsApp de l'école"
resume: "Ce module pilote WhatsApp comme canal de communication officiel de l'école : connexion du compte expéditeur (numéro WhatsApp Business de l'école ou celui prêté par EduEasy), gestion des modèles de ..."
audiences: [school_admin]
---
# 💬 Configuration WhatsApp de l'école

## 🎯 Rôle
Ce module pilote **WhatsApp comme canal de communication officiel** de l'école : connexion du
**compte expéditeur** (numéro WhatsApp Business de l'école ou celui prêté par EduEasy),
gestion des **modèles de messages** (templates approuvés ou messages manuels), **tests
d'envoi**, et **envois en masse** à une liste de destinataires (parents d'une classe, tous
les parents…). Bien configuré, il remplace des **centaines de SMS payants**.

## ✅ Prérequis
1. Être **School Admin**.
2. Avoir **choisi son mode** :
   - **WhatsApp EduEasy** (partagé) : rien à saisir, contactez le Support pour l'activer ;
   - **Votre compte WhatsApp Business** : récupérer **Phone number ID** et **Access token**
     et les saisir dans *08-clés-api-integrations.md*.
3. Accès : menu **WhatsApp** (`whatsapp.index`).

## 🟢 Connecter et tester (étape par étape)
1. Ouvrez **WhatsApp** → **Paramètres** : vérifiez/saisissez le **numéro expéditeur** et les
   identifiants → **Enregistrer** (`whatsapp.settings`).
2. Cliquez **Tester la connexion** (`whatsapp.test-connection`) : validation de l'appariement.
3. Envoyez un **message test** (`whatsapp.test-message`) sur votre propre numéro : vous
   devez le recevoir dans WhatsApp.

## 📝 Gérer les modèles de messages
1. **Templates officiels** : liste (`whatsapp.templates.list`), **modifier** le contenu
   autorisé (`whatsapp.templates.update/{id}`) et **tester** un template
   (`whatsapp.templates.test/{id}`).
2. **Templates manuels** (libres) : **créer** (`whatsapp.manual-templates.store`),
   **modifier** (`whatsapp.manual-templates.update/{id}`), **supprimer**
   (`whatsapp.manual-templates.destroy/{id}`) — la suppression est **définitive** : recréez
   le message si besoin.

## 📤 Envoi en masse (étape par étape)
1. Ouvrez la **liste des destinataires** (`whatsapp.recipients.list`) : parents joignables
   sur WhatsApp.
2. **Cochez** les destinataires (ou sélectionnez une classe).
3. Choisissez le **message/template** → lancez l'**envoi groupé** (`whatsapp.bulk-send`).
4. Consultez les **statuts de remise** dans le journal (*10*).

## ✏️ Modifier / 🔴 Supprimer / ♻️ Restaurer
- **Configuration** : se corrige en enregistrant par-dessus (Modifier).
- **Templates manuels** : suppression **sans corbeille** → **recréez-les** ; gardez une copie
  des textes importants dans un document.
- **Envoi partiel raté** : pas d'annulation possible d'un message WhatsApp **déjà reçu** —
  assumez et envoyez un **message correctif** si nécessaire.

## ⚠️ Bon à savoir
- **Règles WhatsApp** : les messages **commerciaux/hors contexte** peuvent être bloqués par
  Meta si le compte est signalé — gardez des messages **utiles et sobres**.
- **Numéro du parent doit être sur WhatsApp** : la liste des destinataires ne montre que les
  numéros joignables ; les autres reçoivent des **SMS** (voir *09*).
- **Ne changez pas de numéro expéditeur** en pleine campagne de rappels : les parents
  enregistreraient un « inconnu ».
- **Heures d'envoi** : programmez tôt (7h-12h) — un SMS/WhatsApp à 22h agace plus qu'il
  n'informe.
- Les **annonces classiques** (avec option WhatsApp) restent dans le module **Annonces**.
