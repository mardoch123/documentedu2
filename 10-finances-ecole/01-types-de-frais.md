---
id: 10-01-types-de-frais
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-01-types-de-frais
emoji: "🏷️"
titre: "Créer / modifier / supprimer / restaurer un type de frais"
resume: "Un type de frais est une catégorie de paiement utilisée partout dans la facturation : Scolarité, Droits d'inscription, Cantine, Transport, Fournitures, etc."
audiences: [school_admin, staff]
---
# 🏷️ Créer / modifier / supprimer / restaurer un type de frais

## 🎯 Rôle
Un **type de frais** est une **catégorie** de paiement utilisée partout dans la facturation :
*Scolarité*, *Droits d'inscription*, *Cantine*, *Transport*, *Fournitures*, etc. Avant de
pouvoir **créer une grille de frais** ou encaisser, il faut **déclarer ces types**. Cette page
couvre le cycle complet du type de frais : **créer, modifier, supprimer (corbeille),
restaurer**.

## ✅ Prérequis
1. Option « **Fees Management** » + permission « fees-type-list » (création : direction).
2. Accès : menu **Fees → Fees Type** (`fees-type.index`).
   > C'est la **toute première étape** de la configuration des frais : faites-le avant de
   > créer une grille (*02-frais-scolaire-par-classe.md*).

## 🟢 Créer un type de frais (étape par étape)
1. Ouvrez **Fees Type** (sous-titre : *« Créez et administrez les catégories de frais
   utilisées dans toute la facturation de votre école : scolarité, inscription, cantine,
   transport… »*).
2. Dans le bloc **« Create Fees Type »**, saisissez :
   - **« name »** ★ — le nom de la catégorie (ex. « Scolarité 2026 ») ;
   - **description** — précision facultative.
3. Cliquez **« submit »**. Le type apparaît dans la liste (colonnes **Nom, Description,
   Action**).

## ✏️ Modifier un type de frais
1. Sur la ligne du type, cliquez l'**icône Modifier** (colonne Action).
2. La fenêtre **« Edit Fees Type »** reprend **name** ★ et **description**.
3. Corrigez puis **« submit »**.

## 🔴 Supprimer un type de frais (corbeille)
1. Sur la ligne, cliquez l'**icône Supprimer**, puis confirmez.
2. Le type part à la **corbeille** : il disparaît de la liste mais reste **récupérable**.
3. Basculez le sélecteur **« all | Trashed »** (au-dessus du tableau) sur **« Trashed »** pour
   voir les types supprimés.
4. Depuis « Trashed », l'action de **suppression définitive** efface pour de bon.
   > ⚠️ Un type **utilisé dans une grille de frais active** ne doit pas être supprimé :
   > vérifiez avant.

## ♻️ Restaurer un type de frais supprimé
1. Passez la liste en mode **« Trashed »**.
2. Cliquez l'**icône Restaurer** sur le type voulu.
3. Le type **revient dans la liste active** et redevient sélectionnable dans les grilles.

## ⚠️ Bon à savoir
- La liste est un tableau **recherchable / exportable** (boutons Recherche, Colonnes, Rafraîchir,
  Export en haut à droite).
- **Nommez clairement** vos types (« Inscription », « Scolarité T1 », « Cantine ») : ils
  réapparaissent dans chaque grille et chaque reçu.
- Les types servent de **briques** aux grilles de frais (*02*) : préparez-les d'abord.
- **Suppression réversible** : en cas d'erreur, l'onglet « Trashed » + Restaurer sauve la mise.
