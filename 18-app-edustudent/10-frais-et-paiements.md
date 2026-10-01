---
id: 18-10-frais-et-paiements
partie: 18
titre_partie: "Application EduStudent"
app: edustudent
slug: 18-10-frais-et-paiements
emoji: "💳"
titre: "les frais de l'enfant et payer (mobile money, carte, USSD)"
resume: "Écran financier de la famille : voir ce que l'élève doit, paiement en ligne FeexPay/KKiaPay (mobile money, carte), paiement USSD depuis le téléphone, reçus et historique des tran"
audiences: [parent, student, school_admin]
---
# 💳 18.10 — EduStudent : les frais de l'enfant et payer (mobile money, carte, USSD)

## 🎯 Rôle
Écran financier de la famille : voir **ce que l'élève doit**, paiement en ligne
**FeexPay/KKiaPay** (mobile money, carte), paiement **USSD** depuis le téléphone,
**reçus** et **historique** des transactions.

## ✅ Prérequis
1. Être connecté en **parent** (page 18.1) puis sélectionner l'enfant (page 18.3) —
   ou l'élève pour consultation.
2. Que l'école ait créé les **frais** (PARTIE 10) et activé au moins un **moyen de
   paiement en ligne** (page 17.21 côté école).
3. Un compte mobile money actif (MTN/Moov/Orange/Wave…) pour payer par téléphone.

## 🟢 Voir la situation de l'enfant
1. Menu enfant → **« Frais »** (childFees) : total dû, payé, reste — par élève.
2. **« Détail des frais »** (childFeeDetails) : chaque **type de frais** avec ses
   **tranches** (échéances), son statut (payé, partiel, en attente) et — s'il existe —
   le **bandeau de réduction** affichant le net réellement dû.
3. Option **« Régler par tranches successives »** : payer tranche par tranche au lieu
   de tout solder.

## 🟢 Payer en ligne (FeexPay / KKiaPay — étape par étape)
1. Sur le frais ou la tranche : bouton **Payer**.
2. Choisir le moyen (Orange Money, MTN MoMo, Wave, carte…) dans la caisse sécurisée.
3. Confirmer le **numéro** qui reçoit la demande, puis **valider le paiement** sur
   votre téléphone (code PIN mobile money).
4. L'écran affiche **« Sécurisation du paiement… »** puis **« Confirmation en cours »** :
   patientez, ne fermez pas.
5. Si l'écran reste bloqué : bouton **« Recharger le statut »** — la banque a peut-être
   déjà débité, l'app va vérifier.
6. Reçu généré : visible dans **« Mes reçus »** (myReceipts) et dans
   **« Transactions »**.

## 🟢 Payer par USSD (sans Internet de transfert)
1. Écran frais → option **USSD** : l'app montre le **numéro USSD de l'école**
   (par ex. *xxx#) et le **montant** — bouton **« Tout solder (NFCFA) »** pour le total.
2. **Composez** le numéro affiché depuis votre téléphone (l'app peut le faire pour
   vous).
3. Suivez les écrans de l'opérateur (PIN, confirmation).
4. Écran **« Confirmation »** dans EduStudent : saisissez la **référence** du SMS
   opérateur si demandé.
5. La direction **valide** la transaction (page 17.20) : le statut passe alors à
   « payé » — « Historique USSD » (ussdHistory) garde vos tentatives.

## 🟢 Consulter reçus et historique
1. **« Mes reçus »** : chaque paiement avec reçu — consultation, partage PDF/image.
2. **« Transactions »** : le fil de tous vos paiements famille (enfant par enfant).

## ✏️ / 🔴 / ♻️
- Un paiement **ne s'annule pas** de l'app : un double débit ou erreur de tranche se
  signale à l'école (cahier ou message) — l'école corrige sur le web (PARTIE 10).
- **« Recharger le statut »** après un blocage : si le débit est confirmé côté
  opérateur mais pas chez l'école, **ne payez pas deux fois** — attendez la validation
  USSD ou contactez le secrétariat.
- Reçu introuvable : il naît de la **validation école**, pas du seul débit : un
  paiement USSD en attente n'a pas encore de reçu définitif.
- Réduction qui « disparaît » du total : elle a été retirée côté école — vérifiez le
  bandeau de la page 17.22 avec la direction avant de contester un montant.

## ⚠️ Bon à savoir
- Payez **toujours la tranche échue** en priorité : le retard déclenche la pénalité
  configurée par l'école (page 17.22).
- Le paiement **USSD** est asynchrone : comptez la validation de l'école (heures
  ouvrables) avant que le solde s'affiche à jour.
- Les montants sont dans la **devise de l'école** (FCFA) : aucune conversion n'est
  faite.
- Conservez le **SMS de l'opérateur** jusqu'au reçu officiel : c'est votre seule preuve
  entre le débit et la validation.
