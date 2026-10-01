---
id: 14-01-commande-cartes-eleves
partie: 14
titre_partie: "Cartes, certificats & rapports"
app: web
slug: 14-01-commande-cartes-eleves
emoji: "💳"
titre: "Commander des cartes scolaires (cartes d'identité plastifiées)"
resume: "Ce module permet à l'école de commander les cartes d'identité plastifiées des élèves auprès du service d'impression EduEasy : vous choisissez les élèves, le type de carte, vous payez la commande en..."
audiences: [school_admin, staff]
---
# 💳 Commander des cartes scolaires (cartes d'identité plastifiées)

## 🎯 Rôle
Ce module permet à l'école de **commander les cartes d'identité plastifiées des élèves**
auprès du service d'impression EduEasy : vous choisissez les **élèves**, le **type de carte**,
vous **payez** la commande en ligne, puis vous **suivez** sa fabrication et sa livraison.
C'est un service **payant** (facturé par carte). ⚠️ Le menu n'apparaît que pour les écoles
**éligibles au service d'impression** (disponibilité du service selon le pays/réglage
plateforme).

## ✅ Prérequis
1. Être **School Admin** (rôle principal de l'école) — le menu est réservé à ce rôle.
2. Le **service d'impression** doit être **disponible** pour votre école (sinon le menu est
   masqué).
3. Avoir des **élèves avec photos** (la photo figure sur la carte).
4. Un moyen de **paiement mobile** fonctionnel (Fedapay/Paystack/FeexPay selon config).
5. Accès : menu **Commande carte** → **Mes commandes** (`card-orders.index`) /
   **Nouvelle commande** (`card-orders.create`).

## 🟢 Passer une commande (étape par étape)
1. Ouvrez **Commande carte → Nouvelle commande**.
2. Sélectionnez la **classe/section** puis les **élèves** concernés.
3. Choisissez le **type/quantité** de cartes ; une **estimation de livraison** peut être
   demandée (`card-orders.estimate`).
4. **Validez la commande** (`card-orders.store`) → elle est créée en attente de paiement.
5. **Payez** : ouvrez la page de paiement (`card-orders.payment`) puis confirmez
   (`card-orders.process-payment`). Sans paiement, la commande n'est **pas lancée**.

## 🚚 Suivre une commande
1. **Mes commandes** (`card-orders.index`) : liste avec **statut** (en attente, payée, en
   fabrication, livrée…).
2. Cliquez sur une commande pour le **détail et le suivi** (`card-orders.show`).

## ✖️ Annuler une commande
1. Ouvrez la commande (`card-orders.show`).
2. **Annuler** (`card-orders.cancel`) — possible **avant** lancement en fabrication.
   L'annulation change le **statut** : la commande reste visible dans l'historique.

## 🔴 Supprimer une commande de la liste
- Suppression (`card-orders.destroy`) réservée à l'**administrateur** (contrôle de
  permissions) : elle **retire définitivement** la commande de votre liste.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** : une commande supprimée ne revient pas — **repassez une nouvelle
  commande**. Préférez l'**annulation** (qui conserve la trace) à la suppression.

## ⚠️ Bon à savoir
- **Photo obligatoire** : cartes sans photo = qualité ratée ; vérifiez les photos d'élèves
  (*module Élèves*) avant de commander.
- **Payez vite** : une commande non payée **dort** ; la file de fabrication ne démarre
  qu'après paiement.
- **Gardez la preuve** : le suivi (`show`) affiche l'état — prenez-le en capture en cas de
  litige, et contactez le **Support EduEasy** via l'entrée **Support**.
- Les **modèles de cartes** et **types d'impression** sont gérés par l'équipe **EduEasy**
  (plateforme) : demandez-leur un nouveau modèle via le **Support** si besoin.
- Pour **imprimer vous-même** des cartes simples (PDF), voir
  *04-cartes-identite-eleves-personnel.md*.
