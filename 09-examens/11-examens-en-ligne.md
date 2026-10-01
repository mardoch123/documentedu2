---
id: 09-11-examens-en-ligne
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-11-examens-en-ligne
emoji: "💻"
titre: "Examens en ligne (créer, lancer, restaurer)"
resume: "Un examen en ligne est une épreuve passée sur l'application (ordinateur / téléphone) sous forme de QCM / questions, avec un temps limité et une fenêtre de dates d'ouverture."
audiences: [school_admin]
---
# 💻 Examens en ligne (créer, lancer, restaurer)

## 🎯 Rôle
Un **examen en ligne** est une épreuve **passée sur l'application** (ordinateur / téléphone)
sous forme de **QCM / questions**, avec un **temps limité** et une **fenêtre de dates**
d'ouverture. L'élève se connecte, saisit la **clé d'examen**, répond dans le temps imparti ;
les réponses sont **corrigées automatiquement** et le **résultat** est consultable. Cette page
couvre **créer, modifier, supprimer (corbeille) et restaurer** un examen en ligne.

## ✅ Prérequis
1. Option « **Exam Management** » + permissions « online-exam-create/list/edit/delete ».
2. Avoir **classes, sections, matières** et surtout des **questions** prêtes
   (*12-questions-examens-en-ligne.md*).
3. Accès : menu **Online Exam → Gérer les examens en ligne** (`online-exam.index`).

## 🟢 Créer un examen en ligne (étape par étape)
1. Ouvrez **Gérer les examens en ligne** ; le bloc **« Créer un examen en ligne »** est en haut.
2. Renseignez dans l'ordre (les listes s'enchaînent) :
   - **« Class »** ★ — la classe ;
   - **« Class Section »** ★ — la/les section(s) (multi-choix, « Select All » dispo) ;
   - **« Subject »** ★ — la matière (se remplit après la section) ;
   - **« title »** ★ — intitulé de l'examen ;
   - **« exam_key »** ★ — **clé d'examen** générée automatiquement (champ en lecture seule :
     c'est le code que l'élève devra saisir pour démarrer) ;
   - **« duration »** ★ — **durée en minutes** ;
   - **« start_date »** ★ — date/heure **d'ouverture** (sélectionneur date-heure) ;
   - **« end_date »** ★ — date/heure **de fermeture**.
3. **Ajoutez les questions** : après création, utilisez l'action **« Assigner des questions »**
   (page `online-exam.add.questions.index`) pour choisir les questions de l'examen — voir
   *12-questions-examens-en-ligne.md*.
4. **Enregistrez / Submit**. L'examen apparaît dans la liste, avec **durée, date de début,
   date de fin**.
5. Communiquez la **clé d'examen** aux élèves ; l'examen est **passable uniquement entre
   start_date et end_date**.

## 📊 Suivre et consulter les résultats
- La liste montre les **participants** et l'état de chaque examen en ligne.
- Le **résultat** d'un examen en ligne est consultable (`online_exam_result`) : notes
  automatiques des QCM, nombre de participants, etc.

## ✏️ Modifier un examen en ligne
1. Sur la ligne, cliquez l'**icône Modifier**.
2. La fenêtre reprend **durée**, **start_date**, **end_date**, titre, etc.
3. Corrigez puis **enregistrez**.

## 🔴 Supprimer un examen en ligne (corbeille)
1. Sur la ligne, cliquez l'**icône Supprimer**, puis confirmez.
2. L'examen part à la **corbeille** (soft-delete) : il disparaît de la liste normale mais
   reste **récupérable**.
3. Pour voir la corbeille, basculez le sélecteur **« all | Trashed »** (au-dessus du tableau)
   sur **« Trashed »**.
4. Depuis « Trashed », l'action de **suppression définitive** efface pour de bon.

## ♻️ Restaurer un examen en ligne supprimé
1. Basculez la liste sur **« Trashed »**.
2. Cliquez l'**icône Restaurer** sur l'examen voulu.
3. L'examen **revient dans la liste active** avec ses questions et réglages.

## ⚠️ Bon à savoir
- La **clé d'examen** est **générée toute faite** : ne cherchez pas à la taper, donnez-la aux
  élèves.
- **Fenêtre start/end** : hors de cette plage, l'examen n'est **plus accessible** ; réglez une
  marge suffisante.
- **Durée ≠ fenêtre** : la **durée** est le temps de réponse d'un candidat ; la **fenêtre**
  (début→fin) est la période pendant laquelle il peut **démarrer**.
- **Pas de questions = examen vide** : attachez toujours des questions (*12*) avant de lancer.
- La **suppression est réversible** (corbeille), comme pour les examens papier.
