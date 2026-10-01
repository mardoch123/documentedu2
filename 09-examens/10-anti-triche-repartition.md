---
id: 09-10-anti-triche-repartition
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-10-anti-triche-repartition
emoji: "🎯"
titre: "Anti-Triche : répartition automatique des élèves en salles"
resume: "Le module Anti-Triche (Répartition automatisée) place automatiquement les élèves dans des salles d'examen, en tables-bancs de 2 places, en mélangeant les classes (deux voisins ne viennent pas de la..."
audiences: [school_admin]
---
# 🎯 Anti-Triche : répartition automatique des élèves en salles

## 🎯 Rôle
Le module **Anti-Triche** (Répartition automatisée) **place automatiquement les élèves dans
des salles d'examen**, en **tables-bancs de 2 places**, en **mélangeant les classes**
(deux voisins ne viennent pas de la même classe) pour **limiter la fraude**. Il **affecte les
surveillants**, génère un **plan 2D** de la salle, des **étiquettes de table avec QR code**,
les **feuilles d'émargement**, le **planning des surveillants** et les **convocations** des
candidats.

## ✅ Prérequis
1. Avoir **créé les examens** et leur **emploi du temps** (*01*, *04*).
2. Avoir **déclaré les salles et tables-bancs** disponibles (voir « Gérer les Salles & Bancs »).
3. Avoir des **enseignants / surveillants** affectables.
4. Permission « exam-create » / « exam-list ». Accès : menu **Anti-triche → Générer répartition**
   (`exams.seating.index`).

## 🏛️ Étape 1 — Gérer les salles et tables-bancs
1. Depuis **Anti-Triche**, cliquez **« Gérer les Salles & Bancs »** (`exams.seating.halls`).
2. **Ajoutez une salle** : nom, capacité (nombre de **tables-bancs**, chaque banc = **2
   places**), éventuellement affectation à une session.
3. Chaque salle est modifiable / supprimable par ses actions de ligne.
4. La page d'accueil **Anti-Triche** affiche en compteurs : **Salles Disponibles**,
   **Capacité Actuelle** (places / tables-bancs), **Sessions d'Examens**.
   > La **capacité totale** doit être **≥ au nombre d'élèves** à caser, sinon la génération
   > échouera partiellement.

## ⚡ Étape 2 — Générer une répartition
1. Revenez sur **Anti-Triche** ; choisissez l'**« Année Académique »** (filtre en haut).
2. Cliquez **« Générer une Répartition »**.
3. Une fenêtre guidée par **étapes** s'ouvre (notamment **« Règles d'Affectation des
   Surveillants »**, ex. **« Minimum 2 surveillants par salle (Chef de salle + Adjoint) »**).
4. Sélectionnez l'**examen** / la session à répartir, puis validez : le logiciel
   **place les élèves** (tables-bancs de 2, mélange des classes) et **affecte les
   surveillants** selon les règles.
5. Chaque examen affiche alors un nombre **« total_seated_students »** (élèves placés).

## 🗺️ Étape 3 — Voir le plan 2D et exporter
Sur la ligne d'un examen **réparti** (élèves placés > 0) :
1. **« Plan 2D »** (`exams.seating.visualizer`) : ouvre la **vue d'ensemble de la salle** —
   tables-bancs, places occupées, surveillants. Idéal pour vérifier d'un coup d'œil.
2. Menu **Exporter** (dropdown sur la ligne) donne trois PDF :
   - **« Étiquettes Tables (QR Code) »** : numéros de table à coller sur chaque banc ;
   - **« Émargement & Portes »** : feuilles d'émargement par salle ;
   - **« Planning Surveillants »** : qui surveille quelle salle.
3. **Convocation par élève** : une **convocation PDF** (numéro de table + salle) est
   téléchargeable par candidat
   (`exams.seating.export.student-convocation`).
4. **Notifier les élèves** : l'action **« Envoyer les convocations … sur l'application
   mobile »** push la convocation (numéro de table + salle) à **tous les élèves** de
   l'examen (fenêtre de confirmation).

## ✏️ / 🔴 Modifier ou annuler une répartition
- Pour **changer les salles** : modifiez d'abord les salles (« Gérer les Salles & Bancs »,
  édition/suppression de ligne), puis **relancez « Générer une Répartition »** : la nouvelle
  génération **remplace** l'ancienne.
- Pour **ajouter/supprimer une salle** : sur la page Salles, utilisez les actions de ligne
  (mettre à jour / supprimer).
- Il n'y a **pas de corbeille** dédiée aux répartitions : on **relance la génération** ; conservez les
  exports (étiquettes, émargement) avant de régénérer si besoin.

## ⚠️ Bon à savoir
- **Tables-bancs = 2 places** : le moteur « anti-triche » alterne les élèves de **classes
  différentes** sur un même banc — préparez vos salles en conséquence.
- **Capacité insuffisante** = des élèves non placés : vérifiez le compteur « places » avant de
  générer.
- **Minimum 2 surveillants par salle** (chef + adjoint) est une règle recommandée pour la
  validité d'un examen surveillé.
- Les **QR codes des tables** peuvent être scannis le jour J pour **pointer la présence** en
  salle (cohérent avec le module Présence QR).
- Faites les **exports la veille** de l'examen : étiquettes, émargements et convocations
  s'impriment en masse.
