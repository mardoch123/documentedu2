---
id: 11-06-taches
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-06-taches
emoji: "✅"
titre: "Tâches et assignations au personnel"
resume: "Le module Tâches (Tasks) permet de donner un travail à un membre du personnel ou à soi-même, avec une échéance, puis d'en suivre l'avancement (À faire → En cours → Terminée)."
audiences: [school_admin, teacher, staff]
---
# ✅ Tâches et assignations au personnel

## 🎯 Rôle
Le module **Tâches (Tasks)** permet de **donner un travail** à un membre du personnel ou à
soi-même, avec une **échéance**, puis d'en **suivre l'avancement** (À faire → En cours →
Terminée). C'est l'**outil de pilotage interne** de l'école : « préparer la salle pour
vendredi », « relancer les impayés de la 6ème », etc.

## ✅ Prérequis
1. Option « **Staff Management** » + permissions « **task-create** » / « **task-assign** ».
2. Avoir des **enseignants / staff** assignables (ils apparaîtront dans la liste des
   destinataires).
3. Accès : menu **Staff Management → Tasks** (`tasks.index`).

## 🟢 Créer une tâche (étape par étape)
1. Ouvrez **Tasks**, cliquez **« Ajouter »** (`tasks.create`).
2. Renseignez :
   - **Titre (title)** ★ — l'action à réaliser ;
   - **Description** ★ — détails, consignes ;
   - **Date d'échéance (due_date)** ★ — deadline ;
   - **Type** ★ :
     - **Pour moi** (type 1) : tâche que vous vous assignez ;
     - **Assignée** (type 2) : vous **choisissez le destinataire** →
       **« user_id »** ★ obligatoire (« Veuillez sélectionner l'utilisateur »).
3. **Enregistrez** (`tasks.store`). La tâche apparaît dans la liste et chez le destinataire.

## 🔄 Suivre l'avancement
1. Ouvrez **Tasks** : chaque ligne a un **statut** — **À faire / En cours / Terminée**.
2. Le destinataire (ou l'assignant) change le statut via **`tasks.update-status`** (bouton
   d'avancement sur la ligne).
3. Filtrez la liste pour voir **vos tâches**, les **en retard** (échéance dépassée) ou les
   **terminées**.

## ✏️ Modifier une tâche
1. Icône **Modifier** (`tasks.edit`) → corrigez titre, description, échéance, destinataire.
2. **Enregistrez** (`tasks.update`).

## 🔴 Supprimer une tâche
1. Icône **Supprimer** (`tasks.destroy`), confirmez → la tâche **disparaît**.

## ♻️ Restaurer
- ⚠️ Les **tâches ne sont pas restaurables** : une tâche supprimée est **perdue** ; il faut la
  **recréer**. Pour « archiver » sans perdre l'historique, **passez plutôt le statut à
  « Terminée »** au lieu de supprimer.

## ⚠️ Bon à savoir
- **Échéance dépassée** = tâche en **retard** : surveillez-la (code couleur / filtre).
- Une tâche **assignée** nécessite un **destinataire valide** (enseignant/staff actif) ;
  si la personne est **désactivée**, elle ne doit plus être choisie.
- La **permission d'assignation** (« task-assign ») est distincte de la simple création :
  sans elle, on ne peut créer que des tâches **pour soi**.
- Les tâches sont un **suivi interne**, **sans lien** avec la paie ni les notes : elles
  n'affectent pas les bulletins.
- Pour un **suivi visuel par personne**, le tableau se filtre par **destinataire** (qui fait
  quoi, pour quand).
