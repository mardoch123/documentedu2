---
id: 09-01-creer-un-examen-offline
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-01-creer-un-examen-offline
emoji: "📝"
titre: "Créer / modifier / supprimer / restaurer un examen (sur papier)"
resume: "Un examen « offline » (sur papier) est une épreuve classique : composition, devoir ou interrogation écrite en salle."
audiences: [school_admin]
---
# 📝 Créer / modifier / supprimer / restaurer un examen (sur papier)

## 🎯 Rôle
Un **examen « offline »** (sur papier) est une **épreuve classique** : composition, devoir ou
interrogation écrite en salle. Créer l'examen **ouvre le cadre** dans lequel les enseignants
vont ensuite **saisir les notes**, publier les résultats et générer les bulletins. Cette page
couvre tout le cycle de vie de l'examen : **créer, modifier, supprimer (mise à la corbeille)
et restaurer**.

> Le menu **« Offline Exam »** regroupe : Gérer les examens, Anti-Triche, Emploi du temps,
> Notes non publiées, Bulletins, Moyennes de passage, Import des notes, Résultats publiés,
> Notations. Il est visible selon la permission et l'option d'abonnement
> **« Exam Management »**.

## ✅ Prérequis
1. Option d'abonnement « **Exam Management** » activée + permission « exam-create ».
2. Avoir créé : **année scolaire**, **semestre/trimestre par défaut**, **classes/sections**,
   **matières** des classes.
3. Le **semestre courant** doit être sélectionné (l'examen y est rattaché automatiquement).
4. Accès : menu **Offline Exam → Gérer les examens** (`exams.index`).

## 🟢 Créer un examen (étape par étape)
1. Ouvrez **Offline Exam → Gérer les examens**. Le bloc **« Créer »** est en haut.
2. Renseignez :
   - **« Exam Name »** ★ — nom de l'examen (ex. « 1er tempsfort Maths »).
     ⚠️ Le logiciel **préfixe automatiquement** le nom selon le type choisi
     (`Devoir_…` ou `Interrogation_…`) — ne remettez pas le mot vous-même.
   - **« Type d'examen »** ★ — **Devoir**, **Interrogation** ou **Composition**.
   - **« Session Years »** ★ — l'année scolaire (celle par défaut est pré-sélectionnée).
   - **« Classes »** ★ — une ou **plusieurs classes** (liste multi-choix ; « Select All » pour
     toutes). **Une classe = un examen créé** : choisir 3 classes crée 3 examens d'un coup.
   - Facultatif : **Description**, **PV**, **Centre**, **Référence Note de Service N°**,
     **Appréciation générale**, **date de début / fin**, **date limite de dépôt des notes**.
3. Cliquez **« submit »**.
4. Chaque examen apparaît dans la liste, et une **notification** est envoyée aux élèves,
   parents et profs concernés.

## ✏️ Modifier un examen
1. Dans la liste, repérez l'examen, cliquez l'**icône Modifier** (colonne Actions).
   > ⚠️ Le bouton Modifier **n'apparaît que si l'examen n'a pas encore de notes saisies**
   > (statut « non commencé »). Une fois les notes engagées, on ne modifie plus l'examen.
2. Corrigez les champs (nom, type, dates, PV, etc.) puis **enregistrez**.

## 🔴 Supprimer un examen (mise à la corbeille)
1. Sur la ligne de l'examen, cliquez l'**icône Supprimer**, puis **confirmez**.
2. L'examen est **mis à la corbeille** (soft-delete) : il disparaît de la liste normale mais
   reste **récupérable** (voir ♻️ ci-dessous).
3. Pour voir les examens à la corbeille, basculez le sélecteur **« all | Trashed »**
   (au-dessus du tableau) sur **« Trashed »**.
4. **Suppression définitive** : depuis l'onglet « Trashed », l'action de suppression forte
   efface pour de bon — **mais elle échoue si des notes ont déjà été saisies** pour cet
   examen (message « Impossible de supprimer ceci car les notes ont déjà été soumises »).
5. Il existe aussi une **suppression en masse** : cochez plusieurs examens puis l'action
   « bulk-destroy ».

## ♻️ Restaurer un examen supprimé
1. Basculez la liste sur **« Trashed »**.
2. Sur l'examen à récupérer, cliquez l'**icône Restaurer**.
3. L'examen **revient dans la liste active** avec ses notes et son emploi du temps intacts.

## ⚠️ Bon à savoir
- **Un examen par classe** : le nom est copié pour chaque classe sélectionnée ; chaque classe
  a sa propre ligne et ses propres notes.
- **Créer l'examen ne saisit aucune note** : après création, allez dans
  **Emploi du temps** (*04*) puis **Saisir les notes** (*02*).
- La **suppression douce est réversible** ; seule la suppression définitive depuis « Trashed »
  est irrévocable — et encore bloquée si des notes existent.
- La **date limite de dépôt des notes** aide la direction à relancer les profs qui n'ont pas
  encore saisi.
- Pour planifier les horaires des épreuves, voir *04-emploi-du-temps-examens.md*.
