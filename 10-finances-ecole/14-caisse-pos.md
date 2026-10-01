---
id: 10-14-caisse-pos
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-14-caisse-pos
emoji: "🛒"
titre: "Point de vente / caisse (produits, ventes, reçus 58 mm)"
resume: "Le Point de vente (Boutique / Caisse) gère une petite boutique scolaire : un catalogue de produits (fournitures, uniformes, livres, collations…"
audiences: [school_admin, staff]
---
# 🛒 Point de vente / caisse (produits, ventes, reçus 58 mm)

## 🎯 Rôle
Le **Point de vente (Boutique / Caisse)** gère une **petite boutique scolaire** : un
**catalogue de produits** (fournitures, uniformes, livres, collations…) et des **ventes
(commandes)** encaissables, avec **reçu imprimable au format thermique 58 mm**. Le stock se
décrémente à chaque vente.

## ✅ Prérequis
1. Être **School Admin** (ou personnel habilité « product » / caisse) pour la boutique de
   l'école.
2. Avoir **créé des produits** avant de pouvoir les vendre.
3. Une **imprimante thermique 58 mm** (ou une imprimante configurée en 58 mm) pour les reçus.
4. Accès : menu **Boutique → Produits** (`products.index`) et **Commandes** (`orders.index`).

## 📦 Gérer les produits (cycle complet)
1. **Créer** : **Produits** → « Ajouter un produit » (permission `product-create`) →
   formulaire (`products.create`) :
   - **Nom** ★ du produit ;
   - **Prix** ★ en **FCFA** ;
   - **Stock** ★ (quantité disponible) ;
   - **Statut** (`is_active`) — interrupteur **actif / inactif**.
   Puis **Enregistrer** (`products.store`).
2. **Modifier** : icône **Modifier** sur la ligne (`products.edit`) → ajustez prix/stock/
   statut → `products.update`.
3. **Filtrer** : la liste « Liste des Produits » se filtre par **Nom** et **Statut**.
4. **Supprimer** : icône **Supprimer** (`products.destroy`) → ⚠️ le produit est
   **définitivement retiré** (pas de corbeille).

## 🧾 Vendre / encaisser une commande (étape par étape)
1. Ouvrez **Commandes** (`orders.index`) ou lancez une **nouvelle vente** depuis la caisse.
2. Ajoutez les **produits** et quantités ; le **total** se calcule.
3. **Encaissez** (`orders.pay`) — espèces ou **FeexPay** (le webhook
   `webhook.feexpay.orders` confirme le paiement en ligne ; page de succès
   `orders.payment-success`).
4. **Imprimez le reçu** : format **thermique 58 mm**, lisible (nom de l'école, lignes de
   produits, total). Le **stock diminue** d'autant.

## ✏️ Modifier / suivi d'une commande
- **Voir** le détail : `orders.show`.
- **Changer le statut** d'une commande (payée, en préparation, livrée, annulée…) :
  `orders.update-status` (PATCH) ou `orders.update`.

## 🔴 Annuler / supprimer une vente
- Une vente ne se **supprime** pas du catalogue : on **change son statut** en « annulée »
  via `orders.update-status`, et on **réintègre le stock** si nécessaire (via l'édition du
  produit ou un retour).

## ♻️ Restaurer
- **Produits** : ⚠️ **pas de restauration** — un produit supprimé doit être **recréé** (mêmes
  nom/prix). Notez les caractéristiques importantes.
- **Commandes** : pas de suppression définitive côté élève ; on **repose le statut** correct.
- **Statut inactif** : un produit **désactivé** (switch `is_active`) reste dans le catalogue
  et se **réactive** à tout moment — c'est la manière sûre de « retirer » un produit sans le
  perdre (préféré à la suppression).

## ⚠️ Bon à savoir
- **Préférez « inactif » à « supprimer »** : un produit inactif disparaît des ventes mais
  **garde son historique** ; un produit supprimé est **irrécupérable**.
- **Stock** : surveillez le **stock bas** ; la vente d'un produit à **0** peut être bloquée.
- Le **reçu 58 mm** est optimisé pour les **petites imprimantes thermiques** (polices
  agrandies, largeur 220 px) ; pour un reçu A4, voir les reçus de frais (*03*).
- **Prix en FCFA** : le champ Prix attend la monnaie de l'école.
- Ne pas confondre avec les **Revenus** saisis à la main (*11*) : ici la recette vient d'une
  **vente de produit** avec **stock**.
