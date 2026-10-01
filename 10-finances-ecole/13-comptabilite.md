---
id: 10-13-comptabilite
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-13-comptabilite
emoji: "📚"
titre: "Comptabilité : tableau de bord, journal et cantine"
resume: "Le module Comptabilité est la mémoire chiffrée de l'école : il centralise automatiquement toutes les écritures (encaissements des frais, dépenses, revenus, cantine) en débit / crédit, offre un tabl..."
audiences: [school_admin, staff]
---
# 📚 Comptabilité : tableau de bord, journal et cantine

## 🎯 Rôle
Le module **Comptabilité** est la **mémoire chiffrée** de l'école : il **centralise
automatiquement** toutes les écritures (encaissements des frais, dépenses, revenus, cantine)
en **débit / crédit**, offre un **tableau de bord d'analyse en temps réel** et un **Grand
Journal** imprimable/exportable. C'est un écran de **consultation** (lecture seule) : on n'y
saisit rien à la main, tout **provient des autres modules**.

## ✅ Prérequis
1. Avoir déjà généré du mouvement : paiements de frais (*03*), dépenses (*10*), revenus
   (*11*), cantine.
2. Permission de consultation comptable (direction).
3. Accès : menu **Comptabilité** — tableau de bord `accounting.dashboard`, journal
   `accounting.journal`, cantine `accounting.canteen.index`.

## 📊 Tableau de bord comptable (`accounting.dashboard`)
1. Ouvrez **Comptabilité** : **analyse en temps réel** des
   **encaissements / décaissements / soldes**.
2. Filtrez par période **« Du … À … »** (dates) pour une période donnée.
3. Utilisez les boutons **« Imprimer »** et **« Exporter »** pour sortir un état.
4. Les données se rechargent dynamiquement (`accounting.dashboard.data`).

## 📒 Grand Journal (`accounting.journal`)
1. Ouvrez **Journal Général Comptable**.
2. Consultez les **KPI** d'en-tête : **Total Écritures, Validées, En attente, Échouées,
   Volume Réglé**.
3. Le tableau détaille chaque **écriture** (date, libellé, **débit**, **crédit**, source).
4. **« Imprimer »** le journal pour le **registre officiel**.

## 🍽️ Comptabilité Cantine (`accounting.canteen.index`)
- Nécessite l'option « **Canteen Management** ».
- Suit l'argent de la **cantine** : **recherche d'un élève** (`search-students`),
  **dossier financier de l'élève** (`student/{id}`), **encaissement espèces**
  (`pay.cash`) et **confirmation de paiement FeexPay** (`pay.feexpay`).
- Ces mouvements alimentent ensuite le **journal général**.

## ✏️ Modifier / 🔴 Supprimer une écriture
- ⚠️ **En lecture seule** : on ne **crée**, ne **modifie** ni ne **supprime** jamais une
  écriture directement dans la comptabilité.
- Pour **corriger** un montant, il faut corriger **l'opération d'origine** dans son module
  (annuler un paiement en *03*, modifier une dépense en *10*, un revenu en *11*), et
  l'écriture comptable **se reflétera** au prochain calcul.

## ♻️ Restaurer
- **Sans objet** : le journal **archive tout** et ne se vide pas. Aucune restauration ; une
  écriture « échouée » ou « en attente » se **retraite depuis sa source**, pas ici.

## ⚠️ Bon à savoir
- **Débit / Crédit** : chaque mouvement a un sens ; le **solde** = encaissements −
  décaissements. En cas de doute, rapprochez-vous du **Grand Journal** et des **KPI**.
- Les écritures **« En attente »** signalent un paiement **pas encore confirmé** (ex. USSD à
  valider *07*, FeexPay en cours) ; les **« Échouées »** = transactions non abouties.
- La comptabilité **ne double compte pas** : frais (*03*), revenus (*11*), dépenses (*10*),
  cantine et paie y convergent **une seule fois**.
- **Imprimer / Exporter** le journal en fin de mois = votre **pièce comptable** d'archive.
- Le tableau de bord est le meilleur point de départ pour un **reporting de direction**.
