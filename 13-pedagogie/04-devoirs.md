---
id: 13-04-devoirs
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-04-devoirs
emoji: "📝"
titre: "Devoirs (assignments) : créer, déposer, corriger"
resume: "Un devoir (assignment) est un travail demandé aux élèves pour une matière et une classe, avec une date limite et parfois un fichier de consigne."
audiences: [school_admin, teacher]
---
# 📝 Devoirs (assignments) : créer, déposer, corriger

## 🎯 Rôle
Un **devoir** (assignment) est un **travail demandé aux élèves** pour une **matière** et une
**classe**, avec une **date limite** et parfois un **fichier de consigne**. Les **élèves
déposent** leur travail, l'enseignant le **corrige** et met une **note/un retour**. C'est le
cycle **donner → rendre → corriger**.

## ✅ Prérequis
1. Avoir **classes, matières, enseignants** et **élèves** inscrits.
2. Permission « assignment ». Accès : menu **Assignment** (`assignment.index`).

## 🟢 Créer un devoir (étape par étape)
1. Ouvrez **Assignments** → **« Ajouter »** (`assignment.create`).
2. Renseignez : **classe/section**, **matière**, **titre**, **description / consignes**,
   **date limite (due date)**, **barème** éventuel, et le **fichier** de l'énoncé.
3. **Enregistrez** (`assignment.store`). Le devoir est **visible des élèves** de la classe.

## 📤 Déposer un devoir (côté élève)
- L'élève **téléverse son fichier** avant la date limite ; la **remise** est enregistrée
  (vue **`assignment.submission`**, **liste des remises** `assignment.submission.list`).

## ✅ Corriger et noter
1. Ouvrez les **remises d'un devoir** (`assignment.submissionDetails/{id}`).
2. Pour chaque élève, consultez le dépôt
   (`assignment.showSubmissionDetails/{id}/{class}/{subject}`), **corrigez** et **notez**.
3. **Correction en masse** possible (`assignment.bulkAssignmentSubmissionUpdate`) pour saisir
   plusieurs notes d'un coup.

## ✏️ Modifier un devoir
1. Icône **Modifier** (`assignment.edit`) → ajustez consignes/date/barème →
   `assignment.update`.
   > ⚠️ Modifier après dépôt : prudent, certains élèves ont déjà rendu.

## 🔴 Supprimer un devoir
1. Icône **Supprimer** (`assignment.destroy`), confirmez → le devoir **disparaît**.

## ♻️ Restaurer
- ⚠️ Les **devoirs ne sont pas restaurables** (la restauration est désactivée dans ce module) :
  un devoir supprimé est **perdu**, ainsi que l'accès à ses consignes ; il faut le **recréer**.
  Les **dépôts/notes** déjà saisis restent rattachés à l'historique de la matière. **Évitez de
  supprimer un devoir actif** : contentez-vous de changer la date limite.

## ⚠️ Bon à savoir
- **Date limite** : au-delà, le dépôt peut être marqué **en retard** (selon réglage).
- **Un devoir ≠ un examen** : le devoir est un **travail hors évaluation officielle** ; les
  **notes d'examen** relèvent des **Examens** (PARTIE Examens).
- **Fichier d'énoncé** : joignez le sujet (PDF/image) pour éviter les malentendus.
- La **note du devoir** peut **remonter** dans le suivi de l'élève selon la configuration.
- Pour **générer un devoir automatiquement par IA**, voir *05-generateur-devoirs-ia.md*.
