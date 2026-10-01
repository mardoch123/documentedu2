---
id: 10-08-journal-transactions-frais
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-08-journal-transactions-frais
emoji: "🧾"
titre: "Journal des transactions de frais"
resume: "Le Journal des transactions de frais (Fees Transaction Logs) est l'historique complet des paiements en ligne (Mobile Money par lien, carte, FeexPay…"
audiences: [school_admin, staff]
---
# 🧾 Journal des transactions de frais

## 🎯 Rôle
Le **Journal des transactions de frais** (*Fees Transaction Logs*) est l'**historique
complet** des **paiements en ligne** (Mobile Money par lien, carte, FeexPay…) reçus par
l'école. Chaque ligne raconte **une transaction** : qui a payé, combien, via quel moyen, et
si ça a **réussi ou échoué**. C'est un écran **en lecture seule**, indispensable pour
**réconcilier** les recettes et **retrouver** un paiement litigieux.

## ✅ Prérequis
1. Permission « **fees-paid** » (consultation direction/caisse).
2. Avoir déjà reçu des paiements **en ligne** (l'USSD validé manuellement a son propre
   écran, *07*).
3. Accès : menu **Fees → Fees Transaction Logs** (`fees.transactions.log.index`).

## 📋 Consulter le journal (étape par étape)
1. Ouvrez **Fees Transaction Logs** (titre : *« online fees transactions logs »*).
2. Filtrez pour retrouver une transaction :
   - **Statut de paiement** (`payment_status`) : réussi / en attente / échoué ;
   - **Mois** (`month`) ;
   - **Année scolaire** (`session_year`).
3. Lisez le tableau : colonnes **User (payeur), Amount (montant), Payment Gateway
   (moyen : FeexPay, opérateur…), Payment Status (résultat)**.
4. Utilisez la **recherche** et l'**Export** (boutons du tableau) pour sortir une liste
   comptable (CSV).

## 🔎 Retrouver une transaction précise
- Cherchez par **nom du payeur** ou par **montant**.
- Croisez avec le **reçu** de l'élève dans **Student Fees** (*03*) pour confirmer
  l'imputation.

## ✏️ Modifier / 🔴 Supprimer
- ⚠️ Le journal est **en lecture seule** : on ne **modifie** ni ne **supprime** une
  transaction (intégrité comptable). Toute correction passe par le **flux d'origine** :
  - un paiement **à annuler** → annulation dans *03* ;
  - un paiement **en attente/échoué** → à retenter côté parent, ou à valider via *07* si
    c'est de l'USSD.

## ♻️ Restaurer
- **Sans objet** : le journal **conserve tout** et ne se vide pas. Aucune restauration
  n'est nécessaire ni possible ; c'est justement son rôle d'**archive fiable**.

## ⚠️ Bon à savoir
- Une transaction **échouée** n'engage **pas** l'argent : l'élève reste à payer. Invitez le
  parent à **réessayer** ou à payer autrement.
- **FeexPay** apparaît comme `payment_method` / Payment Gateway pour tout paiement en ligne
  traité par ce prestataire.
- Ce journal **ne remplace pas** la **saisie manuelle de recettes** : pour un encaissement
  en espèces à la caisse, voir *03* ; pour une recette hors scolarité, voir **Revenus**
  (*11*).
- Filtre **mois + année scolaire** = la base d'un **état de recette mensuel**.
- En cas de **double débit** signalé par un parent, c'est ici qu'on **prouve** la ou les
  transactions (capture d'écran + export).
