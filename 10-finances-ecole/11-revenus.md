---
id: 10-11-revenus
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-11-revenus
emoji: "💰"
titre: "Revenus : tableau de bord, catégories et saisie"
resume: "Le module Revenus enregistre toute recette qui n'est pas un frais scolaire : location de salle, dons, subventions, vente de matériel, activités, cotisations…"
audiences: [school_admin, staff]
---
# 💰 Revenus : tableau de bord, catégories et saisie

## 🎯 Rôle
Le module **Revenus** enregistre **toute recette qui n'est pas un frais scolaire** : location
de salle, dons, subventions, vente de matériel, activités, cotisations… Comme les dépenses,
il offre un **tableau de bord**, des **catégories de revenu** et la **saisie** ligne à ligne.
Avec *Frais encaissés* (*03*), il forme la **vision complète des recettes** de l'école.

## ✅ Prérequis
1. Permission « **income** » (saisie) et « income-category » (catégories).
2. Avoir **créé au moins une catégorie de revenu** avant de saisir.
3. Accès : menu **Finances → Revenus** ; tableau de bord `income/dashboard`, liste
   (`income.index`), catégories (`income.category.*`).

## 🏷️ Gérer les catégories de revenu (cycle complet)
Catégories rangent les recettes (ex. « Location », « Dons », « Activités »).
1. **Créer** : **Catégories de revenu**, **nom** ★ (+ description), validez.
2. **Modifier** : icône **Modifier**, corrigez, enregistrez.
3. **Supprimer (corbeille)** : icône **Supprimer** → corbeille ; basculez **« all | Trashed »**
   sur **« Trashed »**.
4. **Restaurer** : depuis « Trashed », **Restaurer** → la catégorie revient. ⚠️ Ne supprimez
   pas une catégorie **encore utilisée**.

## 🟢 Saisir un revenu (étape par étape)
1. Ouvrez **Revenus** puis **« Ajouter »** (`income.create`).
2. Renseignez :
   - **session_year** ★ — année scolaire ;
   - **« category »** ★ — catégorie de revenu ;
   - **« title »** ★ — libellé (ex. « Location salle samedi ») ;
   - **reference_no** — référence du document (reçu, virement) ;
   - **« amount »** ★ — montant **FCFA** encaissé ;
   - **« date »** ★ — date de la recette (**jamais future**) ;
   - **description** — détails.
3. **Enregistrez**. Le revenu apparaît dans la liste et le **tableau de bord**.

## 📊 Tableau de bord des revenus
- `income/dashboard` : **totaux des recettes**, **répartition par catégorie** et par période.
- La **liste** est **recherchable / exportable** (Recherche, Colonnes, Rafraîchir, Export).

## ✏️ Modifier un revenu
1. Icône **Modifier** (`income.edit`), corrigez montant/date/catégorie.
2. **Enregistrez**.

## 🔴 Supprimer un revenu
1. Icône **Supprimer**, confirmez.
2. ⚠️ Le revenu est **définitivement effacé** (pas de corbeille pour les revenus).

## ♻️ Restaurer
- **Revenus** : ⚠️ **pas de restauration** — il faut **re-saisir** la ligne perdue. Seules les
  **catégories** sont restaurables (bloc catégories plus haut).

## ⚠️ Bon à savoir
- **Ne saisissez PAS ici les frais scolaires** : les paiements d'élèves vivent dans *03* ;
  ce module est réservé aux **recettes annexes** (sinon vous compteriez double).
- **Date non future** : le champ date refuse le futur.
- Les revenus alimentent la **Comptabilité** (*13*) et le **tableau de bord général**.
- **reference_no** : documentez chaque recette (traçabilité, audit).
- Pour la **caisse / point de vente** (ventes de produits), voir *14-Caisse POS*, distinct
  des revenus saisis manuellement.
