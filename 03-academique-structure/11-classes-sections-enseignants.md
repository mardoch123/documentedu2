---
id: 03-11-classes-sections-enseignants
partie: 3
titre_partie: "Académique : Structure & Matières"
app: web
slug: 03-11-classes-sections-enseignants
emoji: "📘"
titre: "Classes, Sections & Enseignants (Profs par matière)"
resume: "C'est le tableau de affectation de l'école : pour chaque classe/section, on définit - le professeur principal (class teacher) de la section, - et quel enseignant enseigne quelle matière dans quelle..."
audiences: [school_admin]
---
# Classes, Sections & Enseignants (Profs par matière)

## 🎯 Rôle
C'est **le tableau de affectation** de l'école : pour chaque classe/section, on définit
- le **professeur principal** (class teacher) de la section,
- et quel **enseignant enseigne quelle matière** dans quelle classe.

Sans cette page : pas de professeur visible sur les bulletins, emplois du temps impossibles
à générer normalement, saisies de notes non filtrées pour les profs.

## ✅ Prérequis
1. Des **classes + sections** ([07-classes.md](07-classes.md)).
2. Des **matières affectées aux classes** ([08-matieres-de-classe.md](08-matieres-de-classe.md)).
3. Des **enseignants** créés (menu *Teacher* — voir [11-enseignants-personnel](../11-enseignants-personnel/01-liste-enseignants.md)).
4. Permission « class-section-list ».

Accès : menu **Académique → Class Section & Teachers** (ou lien « Profs par matière »
depuis la page Classes).

## 🟢 Définir le professeur principal d'une section
1. Ouvrez la page **Class Section & Teachers**.
2. Filtrez sur la **classe** et la **section** voulues (listes déroulantes en haut).
3. Sur la ligne de la section, cliquez sur l'icône **crayon ✏️** (ou « Assign »).
4. Dans le champ **Class Teacher / Professeur principal**, choisissez l'enseignant
   dans la liste déroulante (recherche possible en tapant son nom).
5. Cliquez sur **Soumettre**. Le nom du prof principal s'affiche sur la ligne.

## 🟢 Affecter un prof à une matière d'une classe
1. Sur la même page (ou l'onglet « Subject Teachers » selon l'écran affiché) :
   sélectionnez **Classe → Section → Semestre → Matière**.
2. Choisissez l'**enseignant** affecté à cette matière pour cette classe.
3. **Soumettre**. La ligne apparaît avec la matière, la classe et le prof.
4. Répétez pour chaque matière (c'est long la première fois — aidez-vous de la
   **Bascule d'année** chaque nouvel an pour reconduire les affectations).

## ✏️ Modifier une affectation
1. Retrouvez la ligne (filtres ou loupe) → icône **crayon ✏️**.
2. Changez l'enseignant ou la matière → **Soumettre**. L'ancien prof perd l'accès
   à la matière, le nouveau l'obtient immédiatement.

## 🔴 Supprimer une affectation
1. Icône **poubelle 🗑** sur la ligne → confirmer.
Effet : la matière reste dans la classe, mais **sans enseignant attitré**.

## ♻️ Restaurer
Cette page propose le filtre **« Trashed »** : ouvrez-le, cliquez sur **restaurer ♻️**
sur la ligne, confirmez. Sinon, recréez simplement la même affectation.

## ⚠️ Bon à savoir
- Un enseignant peut cumuler : prof principal de « 6ème A » **et** prof de maths en « 5ème ».
- Pour les enseignants eux-mêmes, cette page est en **lecture** : ils y voient « mes classes »
  et l'emploi du temps qui en découle.
- Un changement de prof **après** la saisie des notes n'efface pas les notes déjà saisies.
