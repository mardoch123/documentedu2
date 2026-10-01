---
id: 09-04-emploi-du-temps-examens
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-04-emploi-du-temps-examens
emoji: "📅"
titre: "Emploi du temps des examens (calendrier des épreuves)"
resume: "L'emploi du temps d'examen fixe quand et à quelle heure chaque matière est composée, pour un examen donné."
audiences: [school_admin]
---
# 📅 Emploi du temps des examens (calendrier des épreuves)

## 🎯 Rôle
L'**emploi du temps d'examen** fixe **quand et à quelle heure** chaque matière est composée,
pour un examen donné. Il transforme l'examen (simple dossier) en un **vrai calendrier
d'épreuves** : date, heure de début, heure de fin, par matière. C'est aussi ici qu'on définit
la **date limite de dépôt des notes** et qu'on peut **générer le calendrier automatiquement**.

## ✅ Prérequis
1. Avoir **créé l'examen** et choisi sa(ses) **classe(s)** (*01*).
2. La **matière** de la classe doit exister et être rattachée à l'examen.
3. Permission « exam-create » / gestion des examens.
4. Accès : menu **Offline Exam → Emploi du temps** (`exams.timetable`).

## 🟢 Créer l'emploi du temps (étape par étape)
1. Ouvrez **Emploi du temps** ; sélectionnez l'**examen** concerné.
2. En haut, renseignez la **« Exam Result Submission Date »** ★ : la **date limite** à partir
   de laquelle les notes doivent être toutes saisies (sert aux relances de la direction).
3. Sous **« Créer l'emploi du temps »**, ajoutez une ligne **par matière** (bouton
   « add new row » / répéteur) et pour chaque ligne :
   - **Matière** ★ (liste des matières de la classe) ;
   - **Date** de l'épreuve ;
   - **« start_time »** ★ — heure de début ;
   - **heure de fin** (*end_time*) ;
   - éventuellement **salle / type d'épreuve** selon les champs proposés.
4. Cliquez sur **Enregistrer / Soumettre**. Le calendrier de l'examen est enregistré
   (route de mise à jour du timetable).

## ⚡ Générer automatiquement le calendrier
1. Sur la page Emploi du temps, cliquez le bouton vert **« Générer automatiquement »**
   (`Générer automatiquement`).
2. Le logiciel **place les épreuves** (matières, créneaux, dates) selon les règles internes,
   en répartissant les épreuves sur la période de l'examen.
3. **Vérifiez** le résultat, ajustez à la main les conflits, puis **enregistrez**.
   > ⚠️ La génération automatique a besoin que **les semestres/trimestres aient des dates**.
   > Si un trimestre n'a pas de dates de début/fin, le logiciel déduit la période depuis le
   > nom du trimestre ; en cas d'anomalie, renseignez les dates du semestre.

## ✏️ Modifier une épreuve
1. Revenez sur l'**emploi du temps** de l'examen.
2. Changez la **date**, l'**heure de début/fin** ou la matière de la ligne concernée.
3. **Enregistrez** la modification.

## 🔴 Supprimer une épreuve du calendrier
- Sur la ligne de matière concernée, utilisez l'**icône de suppression** de la ligne
  (route `exams.delete-timetable`). La ligne disparaît du calendrier.
- Pour annuler **tout**, supprimez plutôt l'**examen** entier (*01*).

## ♻️ Restaurer
- Il n'y a **pas de corbeille** pour une ligne d'emploi du temps supprimée : **ré-ajoutez la
  ligne** (matière, date, heures) puis enregistrez.
- L'**examen**, lui, reste restaurable depuis l'onglet « Trashed » (*01*).

## ⚠️ Bon à savoir
- **Toutes les matières doivent avoir leur note saisie** avant de pouvoir **publier** les
  résultats : l'emploi du temps liste les épreuves attendues pour la publication (*06*).
- La **date limite de dépôt des notes** n'est pas bloquante : elle sert à relancer les profs.
- Un **conflit d'horaire** (deux matières à la même heure) est à éviter manuellement : la
  génération automatique aide, mais **relisez toujours**.
- Le calendrier alimente les **convocations** imprimables via le module **Anti-Triche** (*10*).
