---
id: 11-05-roles-et-permissions
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-05-roles-et-permissions
emoji: "🔐"
titre: "Rôles & permissions (qui a droit à quoi)"
resume: "Les rôles définissent ce que chaque utilisateur peut faire dans l'application : un Comptable verra les finances, un Surveillant verra les présences, etc."
audiences: [school_admin]
---
# 🔐 Rôles & permissions (qui a droit à quoi)

## 🎯 Rôle
Les **rôles** définissent **ce que chaque utilisateur peut faire** dans l'application :
un *Comptable* verra les finances, un *Surveillant* verra les présences, etc. Un **rôle** =
un **ensemble de permissions** (droits précis sur chaque écran/action). Cette page
(**Role & Permission**) sert à **créer des rôles**, **cocher leurs permissions** et
**les attribuer** aux enseignants/personnel. ⚠️ C'est le **cadre de sécurité** de l'école :
à manipuler avec soin.

## ✅ Prérequis
1. Être **School Admin** (ou rôle habilité « role-create / role-edit / role-delete »).
2. Option « **Staff Management** ».
3. Accès : menu **Staff Management → Role & Permission** (`roles.index`).

## 📖 Concepts simples
- **Permission** = un **droit unitaire** (ex. « teacher-create », « fees-paid »,
  « exam-delete »). Le logiciel en contient **des centaines**, groupées par module.
- **Rôle** = une **collection de permissions** (ex. « Comptable » = toutes les permissions
  Fees + Expense + Income + Payroll).
- **Utilisateur** = **enseignant ou membre du staff** à qui on **attache un rôle**.

## 🟢 Créer un rôle (étape par étape)
1. Ouvrez **Role & Permission**.
2. Cliquez **« Ajouter »** (`roles.create`).
3. Saisissez le **nom du rôle** ★ (ex. « Responsable cantine »).
4. **Cochez les permissions** que ce rôle possède (par module : Teachers, Fees, Exams,
   Leave, Transport…). Tout cocher/décocher par groupe est possible.
5. **Enregistrez** (`roles.store`). Le rôle apparaît dans la liste.

## 👤 Assigner un rôle à une personne
1. Ouvrez la fiche de l'**enseignant** (*01*) ou du **membre du staff** (*04*).
2. Dans le champ **Rôle**, sélectionnez le rôle créé.
3. **Enregistrez** : la personne **voit désormais** exactement les écrans de son rôle.
> Astuce : le menu propose parfois un **changement de mode de rôle** (`switch-role-mode`)
> pour basculer l'affichage entre logiques d'accès.

## ✏️ Modifier un rôle
1. Icône **Modifier** sur le rôle (`roles.edit`).
2. Ajustez nom et **permissions cochées** → `roles.update`.
3. Le changement s'applique **immédiatement** à **tous** les porteurs du rôle.

## 🔴 Supprimer un rôle
1. Icône **Supprimer** (`roles.destroy`), confirmez.
2. ⚠️ **Retirez d'abord le rôle** de toutes les personnes qui le portent (sinon elles se
   retrouvent **sans droits**).

## ♻️ Restaurer
- ⚠️ Les **rôles ne sont pas restaurables** : un rôle supprimé est **perdu** (il faut le
  **recréer** et recocher ses permissions). **Notez** la composition des rôles importants
  avant toute suppression.

## ⚠️ Bon à savoir
- **Moins c'est mieux** : n'attribuez que les permissions **nécessaires** au rôle (principe
  du moindre privilège) — ça protège les données sensibles (frais, bulletins).
- **Ne modifiez pas le rôle « School Admin »** dont vous dépendez : vous pourriez perdre
  l'accès à la configuration.
- Beaucoup d'écrans sont en plus **verrouillés par l'abonnement** de l'école
  (feature « … Management ») : une permission ne suffit pas si le **module n'est pas
  souscrit**.
- **Rôles système** (Super Admin, School Admin, Teacher, Staff) existent déjà ; créez des
  rôles **personnalisés** pour vos besoins spécifiques.
- En cas de « je ne vois pas un menu » : vérifiez d'abord le **rôle/permissions** de la
  personne, puis l'**activation du module**.
