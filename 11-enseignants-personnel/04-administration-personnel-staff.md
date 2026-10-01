---
id: 11-04-administration-personnel-staff
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-04-administration-personnel-staff
emoji: "🏢"
titre: "Gestion du personnel non enseignant (Staff) + import en masse"
resume: "Le Staff regroupe tout le personnel non enseignant : direction adjointe, comptabilité, secrétariat, surveillants, ouvriers, chauffeurs, aides, bibliothèque, infirmerie…"
audiences: [school_admin]
---
# 🏢 Gestion du personnel non enseignant (Staff) + import en masse

## 🎯 Rôle
Le **Staff** regroupe tout le **personnel non enseignant** : direction adjointe,
comptabilité, secrétariat, surveillants, ouvriers, chauffeurs, aides, bibliothèque,
infirmerie… Chaque membre a une **fiche** (identité, poste, rémunération), peut recevoir une
**carte d'identité** et être **importé en masse**. Ce module gère le **cycle complet** :
**créer, modifier, désactiver, supprimer (corbeille), restaurer**, plus l'**import Excel/CSV**
et le **rattachement à la paie**.

## ✅ Prérequis
1. Option « **Staff Management** » + permissions « staff-create / staff-edit / staff-list /
   staff-delete ».
2. Accès : menu **Staff Management → Staff** (`staff.index`).
   > ⚠️ Le **formulaire de création est intégré à la page liste** (pas de page « /create »
   > séparée : `/staff/create` redirige vers `/staff`).

## 🟢 Créer un membre du personnel (étape par étape)
1. Ouvrez **Staff** ; cliquez **« Ajouter »** (formulaire sur la page même).
2. Renseignez : identité (prénom, nom, email **unique**, mobile, sexe, date de naissance,
   adresses), **poste/qualification**, **photo**, **mode de rémunération** (salaire/taux
   horaire) et **statut** (actif/inactif).
3. **Enregistrez** (`staff.store`). Le membre apparaît dans la liste.

## ✏️ Modifier / structure de paie
- Icône **Modifier** sur la ligne → ajuster → `staff.update`.
- **Structure de paie** du membre : `staff.payroll-structure/{id}` (consultation) ;
  modification via `staff/payroll-setting/{id}` (PUT) et suppression via DELETE — ces
  réglages alimentent la **Paie** (*PARTIE 10 — 12-paie*).
- **Carte d'identité** : générer/imprimer (`staff.id-card`, `staff.show.all`,
  `generate-id-card`).

## 📥 Import en masse (Bulk Upload)
1. Bouton **« Bulk upload »** (`staff.create-bulk-upload`).
2. **Téléchargez le modèle** (`staff.bulk-data-sample`) pour avoir les **colonnes exactes**.
3. Remplissez le **CSV** (une ligne = un membre), puis **Importer**
   (`staff.store-bulk-upload`).

## 🔗 Fusionner un compte Staff avec un Enseignant
- Si une personne est **à la fois** enseignant et personnel (ou compte en double), utilisez
  **« Fusionner avec un enseignant »** (`staff.merge-with-teacher`) pour **unifier** les deux
  fiches et **éviter les doublons** d'email.

## ⏸️ Désactiver / 🔴 Supprimer (corbeille) / ♻️ Restaurer
1. **Désactiver** : basculez le **statut** sur la ligne (`staff/{id}/change-status`) — le
   compte est **conservé**, accès coupé. **En masse** : cases à cocher +
   `staff/change-status-bulk`.
2. **Supprimer** : icône **Supprimer** → l'entrée part à la **corbeille** (`staff.trash`).
   Basculez **« all | Trashed »** sur **« Trashed »** pour la voir.
3. **Restaurer** : depuis « Trashed », **Restaurer** (`staff.restore`, remis en changement de
   statut) → le membre **revient actif** avec son historique.

## ⚠️ Bon à savoir
- **Même logique que les enseignants** : statut (désactivation), corbeille, restauration.
- **Email unique** : un email déjà pris (par un prof ou un autre membre) est refusé → d'où
  l'utilité de la **fusion**.
- Les **chauffeurs et aides** de transport relèvent d'un module **séparé** (`driver-helper`,
  voir PARTIE Services) mais suivent la **même mécanique** (import, statut, restore).
- **Paie** : ne payez pas le personnel via Dépenses ; utilisez le module **Paie** nourri par
  la **structure de paie** du membre.
- Le membre peut se connecter (rôle Staff) pour voir ses **congés**, ses **tâches** et ses
  **fiches de paie** (voir *07*, *06*, *09*).
