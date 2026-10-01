---
id: 12-09-bibliotheque-catalogue
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-09-bibliotheque-catalogue
emoji: "📚"
titre: "Bibliothèque : catalogue des livres (+ import)"
resume: "Le catalogue de la bibliothèque range tous les livres possédés par l'école, avec pour chacun un ou plusieurs exemplaires (le même titre, plusieurs copies physiques)."
audiences: [school_admin, staff]
---
# 📚 Bibliothèque : catalogue des livres (+ import)

## 🎯 Rôle
Le **catalogue** de la bibliothèque range tous les **livres** possédés par l'école, avec pour
chacun un ou plusieurs **exemplaires** (le même titre, plusieurs copies physiques). Cette page sert
à **ajouter des livres** (à l'unité ou par **import Excel/CSV**), à **enrichir une fiche**
(auteur, éditeur, ISBN, stock) et à **générer les QR** des exemplaires (*11*).

## ✅ Prérequis
1. Option « **Library Management** » + permissions bibliothèque.
2. Accès : menu **Library** (`library.index`), liste des livres (`library.books.list`).

## 🟢 Ajouter un livre (étape par étape)
1. Ouvrez **Library** ; le **tableau de bord** affiche les compteurs : **livres, exemplaires,
   disponibles, prêts en cours**.
2. **Ajout rapide** (`library.books.quick`) : saisissez **titre**, **auteur**, **éditeur**,
   **ISBN**, **nombre d'exemplaires**, catégorie/emplacement.
3. **Astuce ISBN** : tapez le numéro puis utilisez la **recherche ISBN**
   (`library.isbn.lookup`) pour **pré-remplir** automatiquement titre/auteur/éditeur.
4. **Enregistrez** : le livre entre au catalogue ; ses **exemplaires** deviennent empruntables
   (*10*).

## ✏️ Modifier / consulter une fiche
- **Voir la fiche** du livre (`library.books.show`) : ses **exemplaires**, leur **statut**
  (disponible / emprunté), son **emplacement**.
- **Modifier** : corrigez métadonnées / ajoutez des **exemplaires** depuis la fiche.

## 📥 Import en masse (Excel / CSV)
1. Menu **Library → Import** (`library.import.index`).
2. **Téléchargez le modèle**, remplissez une ligne par livre, **déposez le fichier**
   (dropzone) puis **Importez** (`library.import.upload`).
3. Les livres apparaissent en masse au catalogue — idéal à la **rentrée**.

## 🔎 Retirer / restaurer un livre
- La bibliothèque fonctionne par **statut d'exemplaire** (disponible / perdu / retiré) plutôt
  que par suppression brutale : un exemplaire **abîmé ou perdu** est **marqué comme tel**
  (il sort du stock disponible sans casser l'historique des prêts).
- ⚠️ Il n'y a **pas d'onglet « Trashed » / restauration** côté web pour les livres : un
  exemplaire retiré se **ré-intègre** en **remettant son statut à « disponible »** (ou en
  **ré-ajoutant** un exemplaire). Un livre supprimé par erreur se **recrée** (ou se
  **ré-importe** via le CSV).

## ⚠️ Bon à savoir
- **Livre ≠ exemplaire** : un *livre* est le **titre** ; les *exemplaires* sont les **copies
  physiques**. Le prêt porte sur un **exemplaire**.
- **Générez les QR** des exemplaires (*11*) pour scanner rapidement les prêts/retours.
- **Un bon classement** (catégories, cotes, emplacements) accélère la recherche des élèves.
- La **recherche ISBN** fait gagner un temps précieux sur la **saisie des métadonnées**.
- Les **emprunts, retours et réservations** se gèrent dans *10-bibliotheque-emprunts.md*.
