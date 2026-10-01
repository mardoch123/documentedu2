---
id: 12-10-bibliotheque-emprunts
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-10-bibliotheque-emprunts
emoji: "📖"
titre: "Bibliothèque : emprunts, retours et réservations"
resume: "C'est le guichet de la bibliothèque : prêter un exemplaire à un élève, enregistrer le retour, prolonger un prêt, consulter l'historique d'un élève et ses statistiques, et gérer l"
audiences: [school_admin, staff]
---
# 📖 Bibliothèque : emprunts, retours et réservations

## 🎯 Rôle
C'est le **guichet de la bibliothèque** : **prêter** un exemplaire à un élève, enregistrer le
**retour**, **prolonger** un prêt, consulter l'**historique** d'un élève et ses
**statistiques**, et gérer les **réservations** (un élève réserve un livre indisponible et sera servi dès son
retour).

## ✅ Prérequis
1. Avoir un **catalogue** de livres/exemplaires (*09*).
2. Option « **Library Management** » + permissions prêt.
3. Accès : menu **Library → Loans** (`library.loans.index`) et **Library → Reservations**
   (`library.reservations.index`).

## 🟢 Prêter un exemplaire (étape par étape)
1. Ouvrez **Loans** (emprunts).
2. **Prêt rapide** (`library.loans.loan-quick`) : sélectionnez l'**élève** et l'**exemplaire**
   disponible (scan du **QR** de l'exemplaire si étiquettes *11*), fixez la **date de retour**.
3. **Validez** : l'exemplaire passe en **« emprunté »**, le compteur « prêts en cours » du
   catalogue (*09*) augmente.

## ↩️ Enregistrer un retour
1. Dans **Loans**, utilisez le **retour rapide** (`library.loans.return-quick`) sur l'emprunt
   concerné (scan QR ou sélection).
2. L'exemplaire redevient **« disponible »** et rejoint le stock.

## ⏳ Prolonger un prêt
- Prêt à expirer mais l'élève garde le livre ? **Prolongez** (`library.loans.extend`) : la
  **date de retour** est repoussée (dans la limite autorisée).

## 🗂️ Historique & statistiques d'un élève
- **Historique par élève** (`library.loans.student-history`) : tous ses emprunts/retours.
- **Statistiques des prêts** (`library.loans.statistics`) : titres les plus empruntés,
  volumes, retards — pour piloter le **fonds documentaire**.

## 📌 Réserver un livre indisponible
1. Ouvrez **Reservations** (`library.reservations.index`) ; **recherchez l'élève**
   (`library.reservations.search-students`).
2. **Réserver rapidement** un titre déjà emprunté (`library.reservations.reserve-quick`).
3. Quand l'exemplaire **revient**, le bibliothécaire **honore la réservation**
   (`library.reservations.fulfill`) → l'élève est servi.
4. **Annuler** une réservation devenue inutile (`library.reservations.cancel`).
5. Des **puces de statut** filtrent rapidement les réservations (en attente / servies /
   annulées).

## 🔴 Annuler / ♻️ Restaurer un mouvement
- Un **emprunt** ne se « supprime » pas : on le solde par un **retour**
  (`return-quick`). Une réservation se **cancel** ; elle se **recrée** aussitôt si besoin
  (`reserve-quick`).
- Pas de **corbeille** : les **mouvements** (prêts/retours/réservations) sont un **journal
  d'états** ; l'**historique** reste consultable, rien ne se « restaure » — on **refait**
  l'opération.

## ⚠️ Bon à savoir
- **Retards** : repérez-les via la liste des prêts (date de retour dépassée) et **relancez**
  l'élève ; la **prolongation** (`extend`) évite le blocage.
- **Un exemplaire = un seul emprunt actif** à la fois ; les autres élèves attendent via la
  **réservation**.
- **Servez les réservations dans l'ordre** dès le retour d'un titre (équité).
- Le **scan QR** (*11*) rend prêt/retour **instantanés** et sans erreur de saisie.
- Côté **parent/élève**, l'app mobile permet souvent de **consulter** dispos/reservations —
  mais le **guichet** (prêt/retour) reste à la bibliothèque.
