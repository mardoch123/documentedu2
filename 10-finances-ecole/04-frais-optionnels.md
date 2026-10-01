---
id: 10-04-frais-optionnels
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-04-frais-optionnels
emoji: "➕"
titre: "Frais optionnels (prestations par élève)"
resume: "Les frais optionnels sont des prestations à la carte qu'un élève peut régler sans être obligées : cantine, transport, activités, fournitures, sortie…"
audiences: [school_admin, staff]
---
# ➕ Frais optionnels (prestations par élève)

## 🎯 Rôle
Les **frais optionnels** sont des **prestations à la carte** qu'un élève peut régler sans
être obligées : cantine, transport, activités, fournitures, sortie… Contrairement à la grille
obligatoire, ils se **paient à la demande**, souvent **ligne par ligne**, et se suivent dans
une vue dédiée. Cette page explique **consulter les frais optionnels**, **encaisser** un
frais optionnel et **retirer** un paiement optionnel.

## ✅ Prérequis
1. Avoir **créé des prestations optionnelles** dans une grille de frais (*02*, étape 3).
2. Permission « fees-paid ».
3. Accès : menu **Fees → Optional Fee** (`fees.optional`).

## 🟢 Encaisser un frais optionnel (étape par étape)
1. Ouvrez **Optional Fee** (sous-titre : *« Consultez les paiements de frais optionnels par
   classe et par année scolaire. »*).
2. Filtrez :
   - **Année scolaire** ;
   - **Class Section** ★ ;
   - **Optional Fees** ★ (la prestation à encaisser).
3. La liste des élèves concernés s'affiche (tableau **recherchable / exportable**).
4. Sur l'élève, lancez le **paiement de l'optionnel** (page `fees.optional.index`,
   action de store `fees.optional.store` / `fees.optional-paid.store`) : saisissez le
   **montant** reçu, validez.
5. Le reçu optionnel est édité et le paiement apparaît dans la liste.

## 📋 Consulter l'historique des optionnels
- La même vue sert de **journal des frais optionnels encaissés** par classe/année.
- Boutons du tableau : **Recherche**, **Colonnes**, **Rafraîchir**, **Export** (CSV).

## ✏️ Modifier un paiement optionnel
- On ne « modifie » pas directement un optionnel déjà encaissé : on **retire** le paiement
  puis on le **ré-encaisse** (voir 🔴). Pour un simple ajustement de montant, utilisez
  l'action de mise à jour du paiement sur la ligne.

## 🔴 Retirer un frais optionnel / annuler son paiement
- **Retirer l'optionnel payé** : depuis la fiche de paiement de l'élève, action
  **« remove-optional-fee »** supprime la ligne d'optionnel payée à tort.
- Depuis la grille elle-même (*02*), on peut **supprimer la prestation optionnelle** de la
  grille (ligne du repeater optionnel, ✕) pour ne plus la proposer.

## ♻️ Restaurer
- Pas de **corbeille** pour les paiements optionnels : pour annuler une suppression
  accidentelle, **ré-encaissez** l'optionnel.
- La **prestation optionnelle** retirée d'une grille se ré-ajoute en rechargeant la grille
  (*02*) et en ré-enregistrant.

## ⚠️ Bon à savoir
- Un **frais optionnel ≠ tranche** : l'optionnel est un service ponctuel, la tranche est un
  découpage d'un frais obligatoire (*02*).
- Les **parents** peuvent aussi souscrire/régler certains optionnels depuis leur espace ou
  l'app mobile, selon la configuration.
- **Facturation à la quantité** : si la prestation dépend d'un nombre (mois, repas), la case
  « Quantité » de la grille (*02*) adapte automatiquement le montant.
- Gardez l'**œil sur le statut** (payé / reste) dans **Student Fees** (*03*) pour la vision
  globale des recettes de l'élève.
