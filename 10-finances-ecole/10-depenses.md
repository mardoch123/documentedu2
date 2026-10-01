---
id: 10-10-depenses
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-10-depenses
emoji: "💸"
titre: "Dépenses : tableau de bord, catégories et saisie"
resume: "Le module Dépenses enregistre tout l'argent qui sort de l'école hors paie et hors frais (achats, factures, petit matériel, réparations…"
audiences: [school_admin, staff]
---
# 💸 Dépenses : tableau de bord, catégories et saisie

## 🎯 Rôle
Le module **Dépenses** enregistre **tout l'argent qui sort** de l'école hors paie et hors
frais (achats, factures, petit matériel, réparations…). Il comprend un **tableau de bord**
(visualisation des décaissements), la gestion des **catégories de dépense** et la **saisie**
des dépenses ligne à ligne.

## ✅ Prérequis
1. Permission « **expense** » (saisie) et « expense-category » (catégories).
2. Avoir **créé au moins une catégorie** avant de saisir une dépense.
3. Accès : menu **Finances → Dépenses** ; tableau de bord `expense/dashboard`, liste
   (`expense.index`), catégories (`expense.category.*`).

## 🏷️ Gérer les catégories de dépense (cycle complet)
Les catégories rangent les dépenses (ex. « Fournitures », « Électricité », « Entretien »).
1. **Créer** : ouvrez **Catégories de dépense**, saisissez le **nom** ★ (+ description),
   validez.
2. **Modifier** : icône **Modifier** sur la ligne, corrigez, enregistrez.
3. **Supprimer (corbeille)** : icône **Supprimer** → la catégorie part à la **corbeille**.
   Basculez **« all | Trashed »** sur **« Trashed »** pour la voir.
4. **Restaurer** : depuis « Trashed », cliquez **Restaurer** → la catégorie revient.
   ⚠️ Une catégorie **encore utilisée par des dépenses** ne doit pas être supprimée.

## 🟢 Saisir une dépense (étape par étape)
1. Ouvrez **Dépenses** puis bouton **« Ajouter »** (`expense.create`).
2. Renseignez le formulaire :
   - **« category »** ★ — la catégorie de dépense ;
   - **« title »** ★ — libellé court (ex. « Achat ramettes papier ») ;
   - **« ref_no »** — numéro de référence/facture (facultatif mais recommandé) ;
   - **« amount »** ★ — montant **FCFA** décaissé ;
   - **« date »** ★ — date de la dépense (**jamais une date future**) ;
   - **description** — détails ;
   - **session_year** — année scolaire (par défaut l'année active).
3. **Enregistrez**. La dépense apparaît dans la liste et dans le **tableau de bord**.

## 📊 Tableau de bord des dépenses
- `expense/dashboard` : **vue d'ensemble** des décaissements (totaux, répartition par
  catégorie, périodes). Utile pour le **pilotage budgétaire**.
- La **liste** des dépenses est **recherchable / exportable** (Recherche, Colonnes,
  Rafraîchir, Export).

## ✏️ Modifier une dépense
1. Icône **Modifier** sur la ligne (`expense.edit`).
2. Corrigez montant, date, catégorie… puis **Enregistrez**.

## 🔴 Supprimer une dépense
1. Icône **Supprimer** sur la ligne, confirmez.
2. ⚠️ La dépense est **définitivement effacée** (pas de corbeille pour les dépenses).

## ♻️ Restaurer
- **Dépenses** : ⚠️ **pas de restauration** — une dépense supprimée est **perdue** ; il faut
  la **re-saisir** (notez les références). Seules les **catégories** sont restaurables
  (voir plus haut, ♻️ du bloc catégories).

## ⚠️ Bon à savoir
- **Date non future** : le champ date refuse une date dans le futur — saisissez la date
  réelle du décaissement.
- **La paie** du personnel ne passe **pas** ici : elle a son module dédié (*12-Paie*).
- Les dépenses alimentent le **Grand Journal / la Comptabilité** (*13*).
- **Référence (`ref_no`)** = votre meilleure défense en cas d'audit : documentez chaque
  sortie.
- Une dépense mal catégorisée fausse les **statistiques du tableau de bord** : choisissez
  la bonne catégorie.
