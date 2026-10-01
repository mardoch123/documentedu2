---
id: 09-05-notes-non-publiees
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-05-notes-non-publiees
emoji: "👁️"
titre: "Consulter les notes non publiées (contrôle avant diffusion)"
resume: "Les notes non publiées sont les notes déjà saisies mais pas encore visibles des familles."
audiences: [school_admin, teacher]
---
# 👁️ Consulter les notes non publiées (contrôle avant diffusion)

## 🎯 Rôle
Les **notes non publiées** sont les notes **déjà saisies mais pas encore visibles des
familles**. Cette page sert de **salle de contrôle** : la direction et les profs vérifient ce
qui a été saisi, matière par matière, examens par examens, **avant** de décider de publier.
Rien n'est visible des élèves/parents tant que l'examen n'est pas publié.

## ✅ Prérequis
1. Avoir **saisi des notes** (*02* ou *03*).
2. Permission « view-exam-marks ».
3. Accès : menu **Offline Exam → Notes non publiées** (`exam.view-marks`).

## 🟢 Consulter les notes avant publication (étape par étape)
1. Ouvrez **Notes non publiées** (titre affiché « Manage Exams »).
   Sous-titre : *« Sélectionnez un examen pour consulter et gérer les notes saisies. »*
2. Filtrez la liste :
   - **Année scolaire** (Session Year) ;
   - **Médium / langue** (medium) — filtre « all » par défaut.
3. La **« Liste des examens »** s'affiche avec, pour chaque examen, la colonne
   **« marks_submission_status »** (statut de saisie des notes) : on voit immédiatement
   **quelles matières ont leurs notes** et lesquelles **manquent encore**.
4. Cliquez sur l'examen voulu pour **voir le détail des notes** saisies par élève/matière
   (route `exam.view-marks-list`).

## ✏️ Compléter / corriger une note depuis ici
- Cette page **consulte** ; pour **modifier**, reprenez la **saisie des notes** (*02*) avec la
  même classe / examen / matière : la correction s'applique et revient ici.

## 🔴 Supprimer depuis cette vue
- Il n'y a **pas de suppression d'une note** depuis la vue « non publiées » : on corrige en
  re-saisissant (*02*, dernière valeur gagne) ou on supprime l'**examen** entier (*01*).

## ♻️ Restaurer
- Pas de corbeille propre à cette vue. Seul l'**examen** est restaurable via « Trashed » (*01*).

## ⚠️ Bon à savoir
- Le **statut de saisie** est votre checklist avant publication : un examen ne peut être
  **publié que si toutes les matières ont leurs notes** (sinon message « Les notes ne sont
  pas encore téléchargées pour tous les sujets » → voir *06*).
- « **Non publiées** » ne veut pas dire « enregistrées à moitié » : les notes sont **bien
  stockées**, simplement **masquées** aux familles jusqu'à publication.
- Contrôlez ici les **coquilles** (note > barème, élève oublié) **avant** de publier : une
  fois publié, les familles voient les notes.
- Quand tout est prêt, passez à **Publier les résultats** (*06-publier-resultats.md*).
