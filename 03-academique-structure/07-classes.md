---
id: 03-07-classes
partie: 3
titre_partie: "Académique : Structure & Matières"
app: web
slug: 03-07-classes
emoji: "📘"
titre: "créer, modifier, supprimer, restaurer"
resume: "Une classe est le niveau d'étude de vos élèves : « CP », « 6ème », « Terminale C »…"
audiences: [school_admin]
---
# Les Classes — créer, modifier, supprimer, restaurer

> ⭐ **CETTE PAGE EST L'EXEMPLE TYPE** de toutes les autres : elle montre le cycle complet
> d'une fiche dans EduEasy (création → modification → suppression → restauration).

## 🎯 Rôle
Une **classe** est le niveau d'étude de vos élèves : « CP », « 6ème », « Terminale C »…
Chaque classe regroupe des **sections** (A, B, C), fonctionne dans un **médium**
(Français, Bilingue), éventuellement une **filière** et un **service** (Shift),
et contient des **semestres** pour les notes.

## ✅ Prérequis (à faire DANS cet ordre avant la première classe)
1. Avoir créé au moins un **Médium** → [01-mediums.md](01-mediums.md)
2. Avoir créé vos **Sections** (A, B, C…) → [02-sections.md](02-sections.md)
3. (Secondaire) Avoir créé vos **Filières** → [05-filieres.md](05-filieres.md)
4. (Optionnel) Avoir créé vos **Services** → [06-services-shifts.md](06-services-shifts.md)
5. Votre rôle doit avoir la permission **« Class »** (menu Académique).

Accès : menu **Académique → Class**.

## 🟢 Étape 1 — CRÉER une classe
1. Sur la page **Gestion des classes**, descendez jusqu'au cartouche
   **« Créer une classe »**.
2. **Medium** ★ (obligatoire) : cochez le bouton de la langue d'enseignement de la classe.
3. **Nom** ★ (obligatoire) : tapez le niveau, ex. `6ème` ou `Terminale C`.
   Évitez d'inclure la lettre de section (le champ Section le fait déjà).
4. **Shift** (facultatif) : choisissez le service dans la liste déroulante
   (laissez « --- Sélectionner --- » si vous n'avez qu'un seul service).
5. **Stream / Filière** (facultatif) : sélectionnez une ou plusieurs filières
   (vous pouvez en choisir plusieurs avec Ctrl+clic).
6. **Sections** (facultatif mais recommandé) : cochez les lettres de sections que cette
   classe doit avoir. Si vous avez choisi des filières, une ligne de cases apparaît
   **pour chaque filière**.
7. **Include Semesters** : cochez cette case pour que les **semestres/trimestres**
   soient créés automatiquement pour chaque section. Fortement recommandé.
8. Cliquez sur le bouton **Soumettre** (à droite, en bas du formulaire).
   💡 Le bouton **Réinitialiser** efface le formulaire sans rien enregistrer.
9. Vérifiez : le message de succès apparaît et votre classe est **dans la liste**
   « Liste des classes », avec ses sections et la colonne « Semester = Yes ».

> 🔁 Astuce : créer plusieurs sections d'un coup est possible (case à cocher multiples) —
> « 6ème A », « 6ème B », « 6ème C » naissent en une seule soumission.

## ✏️ Étape 2 — MODIFIER une classe
1. Dans la **Liste des classes**, retrouvez la ligne (recherche possible via la loupe
   au-dessus du tableau).
2. Cliquez sur l'icône **crayon ✏️** de la colonne **Action**.
3. La page de modification s'ouvre avec les valeurs actuelles déjà remplies.
4. Modifiez ce qui doit l'être (nom, sections cochées/décochées, médium…).
   ⚠️ Ne décochez pas une section qui contient déjà des élèves.
5. Cliquez sur **Soumettre / Mettre à jour**.

## 🔴 Étape 3 — SUPPRIMER une classe
1. Dans la liste, icône **poubelle 🗑** sur la ligne de la classe.
2. Une fenêtre demande « Voulez-vous vraiment supprimer ? » → cliquez sur **OK**.
3. La classe **disparaît de la liste « All »** mais n'est pas détruite :
   elle rejoint la **corbeille**.

⚠️ Avant de supprimer une classe :
- Déplacez ou supprimez ses **élèves** (sinon ils se retrouvent sans classe) ;
- Vérifiez qu'aucun **emploi du temps**, **examen** ou **frais** important n'y est rattaché ;
- Une classe supprimée reste liée à des données invisibles : si vous la recréez avec le
  même nom, les anciens bulletins peuvent réapparaître — c'est voulu, pas un bug.

## ♻️ Étape 4 — RESTAURER une classe supprimée
1. En haut de la liste des classes, cliquez sur le filtre **« Trashed »** (Corbeille) —
   à côté du filtre « All ».
2. Seules les classes supprimées s'affichent. Un message mémo est affiché :
   « Les classes supprimées restent accessibles via le filtre Corbeille : vous pouvez
   les restaurer en un clic. »
3. Sur la classe à récupérer, cliquez sur l'icône **restaurer ♻️** (colonne Action).
4. Confirmez. Repassez sur **« All »** : la classe est revenue **avec tous ses élèves,
   sections et semestres d'origine**.

## 🔍 Étape 5 — FILTRER et EXPORTER la liste
- **Filtre Medium** (au-dessus du tableau) : n'affiche que les classes d'une langue.
- **Loupe** : recherche instantanée par nom de classe.
- **Icône Export** : télécharge la liste complète au format Excel/CSV.
- **Roue ↻** : recharge les données.
- **Colonnes** : affiche/masque des colonnes du tableau.

## ⚠️ Bon à savoir
- Les liens rapides en haut de page (« Matières de classe », « Profs par matière »,
  « Référentiel des matières ») ouvrent les modules liés à la classe — voyez les pages
  [08](08-matieres-de-classe.md), [11](11-classes-sections-enseignants.md).
- Le **nom de la classe + la section** s'affichent ensemble partout (ex. « 6ème - A ») :
  c'est ainsi que les reconnaîtrez dans les listes déroulantes des autres modules.
- Le passage de tous les élèves d'une classe vers la classe supérieure se fait avec
  la **Bascule d'année** ou la **Promotion en masse** — voir
  [04-academique-outils-ia/02-bascule-annee.md](../04-academique-outils-ia/02-bascule-annee.md).
