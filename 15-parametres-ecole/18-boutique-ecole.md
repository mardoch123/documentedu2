---
id: 15-18-boutique-ecole
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-18-boutique-ecole
emoji: "🛒"
titre: "Boutique de l'école : produits et commandes"
resume: "Votre école peut vendre des articles (uniformes, livres, fournitures, cartables…"
audiences: [school_admin]
---
# 🛒 Boutique de l'école : produits et commandes

## 🎯 Rôle
Votre école peut **vendre des articles** (uniformes, livres, fournitures, cartables…) via sa
**boutique en ligne** intégrée : vous créez le **catalogue de produits** (prix, stock, photo),
les **parents commandent**, vous suivez chaque **commande** (en attente → payée → expédiée),
encaissez par **mobile money** et gérez les **stocks** sans double saisie.

## ✅ Prérequis
1. Être **School Admin** (ou personnel autorisé sur la caisse).
2. Avoir configuré les **moyens de paiement** (*03*) pour l'encaissement en ligne.
3. Accès : menus **Produits** (`products.index`) et **Commandes** (`orders.index`) ; la
   **caisse POS** (*PARTIE 10-14*) partage le même catalogue.

## 🟢 Créer un produit (étape par étape)
1. Ouvrez **Produits** → **« Ajouter »**.
2. Renseignez :
   - **Nom** du produit (obligatoire) ;
   - **Description** (tailles, matières…) ;
   - **Prix** (obligatoire, ≥ 0) ;
   - **Stock** initial (quantité disponible) ;
   - **Photo** (jpeg/png, max 2 Mo) ;
   - **Actif/Inactif** (un produit inactif disparaît de la vitrine).
3. **Enregistrez** (`products.store`).

## 🛍️ Traiter une commande (étape par étape)
1. Ouvrez **Commandes** (`orders.index`) : liste avec **statut** et **montant**.
2. Cliquez une commande (`orders.show`) : articles, quantités, coordonnées du parent.
3. **Paiement** :
   - le parent paie en ligne depuis sa commande (`orders.pay` → succès `orders.payment-success`,
     confirmation automatique par webhook du prestataire) ;
   - ou vous marquez le **paiement encaissé autrement** puis changez le **statut**
     (`orders.update-status` : en attente → payée → expédiée → livrée / annulée).
4. **Imprimez** le bordereau pour la préparation colis.

## ✏️ Modifier / 🔴 Supprimer
- **Produit** : `products.edit` → corrigez prix/stock/photo → `products.update`.
  Pour **retirer sans effacer** : passez le produit **inactif** (historique conservé).
- **Supprimer un produit** (`products.destroy`) : ⚠️ **définitif, sans corbeille** —
  préférez « inactif » si des commandes passées y sont liées.
- **Commandes** : elles ne se **suppriment pas** (traçabilité) ; une erreur se corrige par le
  **statut annulée** (`orders.update` / `update-status`).

## ♻️ Restaurer
- **Pas de corbeille** ici : produit supprimé = **recréer** le produit (notez les
  caractéristiques) ; commande annulée = le parent **repasse** commande, ou vous **replacez**
  le statut à « en attente ».

## ⚠️ Bon à savoir
- **Le stock se décrémente** à la commande : inventoriez régulièrement (collez
  `stock physique` vs système).
- **Prix ≠ frais de scolarité** : la boutique est un **commerce ponctuel** ; les frais
  scolaires restent au module *Frais* (PARTIE 10).
- **Photos nettes** = 2× plus de ventes : l'uniforme se choisit à l'image.
- **Frais de livraison** : si vous en demandez, ajoutez-les dans la **description** ou
  discutez-en avec le Support pour l'affichage.
- Le **POS de la caisse** et la **boutique** partagent le catalogue : un produit créé ici est
  vendable au comptoir.
