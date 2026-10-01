---
id: 03-03-matieres
partie: 3
titre_partie: "Académique : Structure & Matières"
app: web
slug: 03-03-matieres
emoji: "📘"
titre: "Les Matières (référentiel général)"
resume: "La page Subject contient la liste de toutes les matières possibles de l'école : Mathématiques, Français, SVT, Anglais…"
audiences: [school_admin]
---
# Les Matières (référentiel général)

## 🎯 Rôle
La page **Subject** contient la **liste de toutes les matières possibles** de l'école :
Mathématiques, Français, SVT, Anglais… avec leur code, leur médium et leur type
(théorique ou pratique). C'est le réservoir dans lequel chaque classe puise ses matières.

## ✅ Prérequis
- Avoir déjà créé au moins un **médium** (voir [01-mediums.md](01-mediums.md)).
- Accès : menu **Académique → Subject**. Permission « subject-list ».

## 🟢 Créer une matière
1. Menu **Académique → Subject**.
2. Dans le formulaire du haut de page, remplissez :
   - **Medium** ★ : cochez la langue d'enseignement (Français, Bilingue…) ;
   - **Nom** ★ : ex. `Mathématiques` ;
   - **Type** : **Theory** (théorique) ou **Practical** (pratique — travaux pratiques, sport,
     informatique…) ;
   - **Code** : abréviation courte ex. `MATH` (utilisé dans les bulletins et exports) ;
   - **Couleur** : couleur du badge de la matière (emplez le sélecteur ou un code
     comme `#4F46E5`) — utile dans les emplois du temps ;
   - **Image** (facultatif) : icône illustrant la matière.
3. Cliquez sur **Soumettre**. La matière apparaît dans la liste.

## ✏️ Modifier une matière
1. Dans la liste, icône **crayon ✏️** de la colonne Action.
2. La fenêtre de modification reprend les mêmes champs ; corrigez puis **Soumettre**.

## 🔴 Supprimer une matière
1. Icône **poubelle 🗑** sur la ligne → confirmer.
2. La matière passe en corbeille (filtre **« Trashed »** en haut de la liste).

⚠️ Si la matière est déjà affectée à des classes (page « Class Subject ») ou planifiée,
ces liens cesseront d'être affichés. Supprimez plutôt à la fin de l'année.

## ♻️ Restaurer une matière supprimée
1. Cliquez sur le filtre **« Trashed »**.
2. Icône **restaurer ♻️** sur la matière → confirmez → retour dans la liste « All ».

## ⚠️ Bon à savoir
- Utilisez le **filtre par matière** au-dessus du tableau pour retrouver une ligne dans
  une longue liste, ou la recherche (loupe) du tableau.
- Une matière = une seule fois dans ce référentiel. « Mathématiques 6ème » et
  « Mathématiques Terminale » partagent normalement la même matière ; c'est la page
  **Class Subject** qui fait la différence entre classes.
- Le **code** et la **couleur** sont rarement modifiés après coup : soignez-les à la création.
