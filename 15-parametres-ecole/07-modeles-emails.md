---
id: 15-07-modeles-emails
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-07-modeles-emails
emoji: "✉️"
titre: "Modèles d'emails envoyés aux parents/élèves"
resume: "L'application envoie des emails automatiques : confirmation d'admission, rappel de frais, avis d'absence, notification de bulletin…"
audiences: [school_admin]
---
# ✉️ Modèles d'emails envoyés aux parents/élèves

## 🎯 Rôle
L'application envoie des **emails automatiques** : confirmation d'admission, rappel de frais,
avis d'absence, notification de bulletin… Cette page vous laisse **personnaliser le sujet et
le texte de ces emails** — votre ton, vos formules, votre signature — pour que les messages
portent **l'identité de l'école** au lieu d'un texte générique.

## ✅ Prérequis
1. Être **School Admin**.
2. Une **configuration email** fonctionnelle (sinon les emails ne partent pas — côté
   plateforme, voir Support).
3. Accès : **Paramètres → Email Templates** (`school-settings.email.template`).

## 🟢 Personnaliser un modèle (étape par étape)
1. Ouvrez **Email Templates** : la liste des **types de messages** automatiques.
2. Cliquez sur le **type voulu** (ex. *rappel de frais*, *bienvenue*).
3. Modifiez :
   - le **sujet** de l'email ;
   - le **corps du message**.
   ⚠️ **Conservez intactes les variables entre accolades** (ex. `{student_name}`,
   `{amount}`, `{school_name}`) : c'est le système qui les remplace par les vraies infos au
   moment de l'envoi.
4. **Enregistrez** (`school-settings.email-template.update`, verbe PUT).
5. **Testez** en déclenchant un envoi réel (ex. créer une notification de test).

## ✏️ Modifier à nouveau
1. Reprenez le même modèle, ajustez le texte, **enregistrez**. Le nouveau texte s'applique
   aux **envois futurs** (les emails déjà partis ne changent pas).

## 🔴 Supprimer / ♻️ Restaurer
- Les modèles **ne se suppriment pas** (ils sont nécessaires au système). Pour « restaurer »
  un texte d'origine mal modifié : **redonnez le libellé par défaut** au Support EduEasy ou
  remettez votre copie conservée, puis enregistrez.
- 💡 **Astuce** : avant toute grande modification, **copiez-collez l'ancien texte** dans un
  document de travail.

## ⚠️ Bon à savoir
- **Variables cassées = email invalide** : si vous effacez `{amount}`, le parent verra un
  message sans montant. Touchez **autour** des variables, pas dedans.
- **Restez courts et clairs** : les parents lisent sur téléphone ; une phrase par idée.
- **Orthographe** : relisez-vous — ces emails engagent l'image de l'école.
- Les **SMS/WhatsApp** ont leurs propres modèles (*hub notifications, 09* et *11*) : ici
  uniquement l'**email**.
- **Greffes de signature** : ajoutez nom du directeur et téléphones en bas du modèle.
