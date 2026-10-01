---
id: 12-08-transport-depenses
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-08-transport-depenses
emoji: "⛽"
titre: "Transport : dépenses (carburant, entretien, péages…)"
resume: "Le module Dépenses de transport enregistre tout ce que coûte l'exploitation du parc : carburant, réparations, péages, assurance, nettoyage, primes chauffeurs…"
audiences: [school_admin, staff]
---
# ⛽ Transport : dépenses (carburant, entretien, péages…)

## 🎯 Rôle
Le module **Dépenses de transport** enregistre **tout ce que coûte l'exploitation** du parc :
**carburant**, **réparations**, **péages**, **assurance**, **nettoyage**, primes
chauffeurs… Il permet de **suivre le coût réel** du transport et de le **comparer aux
recettes** (frais de transport des élèves) pour juger de sa **rentabilité**.

## ✅ Prérequis
1. Option « **Transport Management** » (et/ou « Expense ») + permissions dépense transport.
2. Avoir un **parc** (véhicules/lignes) pour rattacher chaque dépense.
3. Accès : menu **Transport → Transportation Expense** (`transportation-expense.index`).

## 🟢 Saisir une dépense de transport (étape par étape)
1. Ouvrez **Transportation Expense**, cliquez **« Ajouter »** (`transportation-expense.create`).
2. Renseignez :
   - **Véhicule / ligne** concerné ;
   - **Type / poste** de dépense (carburant, réparation, péage…) ;
   - **Montant** (FCFA) ;
   - **Date** de la dépense ;
   - **Description / référence** (n° de facture, ticket).
3. **Enregistrez** (`transportation-expense.store`). La dépense s'ajoute au **coût du
   transport** et alimente la **comptabilité**.

## 📊 Suivi & rentabilité
- La liste, **recherchable / exportable**, permet de **cumuler les dépenses** par véhicule,
  par période ou par poste.
- Croisez **dépenses de transport** (cette page) et **recettes** (frais de transport,
  *05*) pour obtenir la **marge** de chaque ligne.

## ✏️ Modifier une dépense
1. Icône **Modifier** (`transportation-expense.edit`) → corrigez montant/date/poste →
   `transportation-expense.update`.

## 🔴 Supprimer une dépense
1. Icône **Supprimer** (`transportation-expense.destroy`), confirmez.
2. ⚠️ La dépense est **retirée** du calcul des coûts.

## ♻️ Restaurer
- ⚠️ Les **dépenses de transport ne sont pas restaurables** (pas de corbeille) : une dépense
  effacée doit être **re-saisie**. Conservez vos **références de factures** pour pouvoir les
  recréer exactement.

## ⚠️ Bon à savoir
- **Rattachez chaque dépense à un véhicule/ligne** : sans ça, le **coût par bus** est
  impossible à calculer.
- Les dépenses de transport **ne passent pas** par le module **Dépenses général** (*PARTIE
  10 — 10-depenses*) : elles ont **leur circuit propre** pour la **rentabilité transport**.
- **Date réelle** du décaissement (pas de date future) pour un suivi fiable.
- Enregistrez les **numéros de tickets/factures** en description : c'est votre preuve en cas
  d'audit (d'autant qu'il n'y a pas de restauration).
- Pour une **vue consolidée** de toutes les sorties d'argent, regardez la **Comptabilité**
  (*13*) qui agrège les écritures.
