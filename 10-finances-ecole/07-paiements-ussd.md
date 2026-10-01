---
id: 10-07-paiements-ussd
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-07-paiements-ussd
emoji: "📱"
titre: "Suivre les paiements USSD / Mobile Money"
resume: "Beaucoup de parents paient depuis leur téléphone (USSD, Orange Money, MTN MoMo, Wave, Moov Money…"
audiences: [school_admin, staff]
---
# 📱 Suivre les paiements USSD / Mobile Money

## 🎯 Rôle
Beaucoup de parents paient **depuis leur téléphone** (USSD, Orange Money, MTN MoMo,
Wave, Moov Money…). Ces paiements arrivent dans l'application **en attente de
vérification**. Cette page (**Paiements USSD**) sert à **contrôler, valider ou rejeter**
ces règlements : une fois **validés**, l'élève est **considéré comme ayant payé** et le
reçu est émis. C'est le **guichet de confirmation** de l'école.

## ✅ Prérequis
1. Avoir **configuré les comptes USSD / Mobile Money** de l'école (Paramètres →
   Mobile Money, compte par opérateur/pays).
2. Permission « **fees-paid** ».
3. Accès : menu **Fees → Paiements USSD** (`fees.ussd-payments.index`).

## 🟢 Valider un paiement USSD (étape par étape)
1. Ouvrez **Paiements USSD** (titre : *« Paiements USSD & Mobile Money »*).
2. Regardez le **KPI « À Valider »** : c'est le nombre de règlements **en attente**.
3. Filtrez si besoin via **`filter_status`** (À valider / Validés / Rejetés).
4. Repérez la ligne : colonnes **Élève, Parent, Montant** (+ opérateur, référence).
5. Ouvrez le détail (`fees.ussd-payments.show`) et **vérifiez** que l'argent est bien reçu
   sur le compte de l'école.
6. Cliquez **« Valider »** (`fees.ussd-payments.validate`). Le paiement est **confirmé**,
   le **reste à payer** de l'élève diminue et le **reçu** est généré.

## 🔴 Rejeter un paiement USSD
1. Sur une ligne douteuse (montant faux, référence introuvable), cliquez **« Rejeter »**
   (`fees.ussd-payments.reject`).
2. Le paiement passe en statut **rejeté** : il **n'est pas compté**, le frais reste dû.
3. Prévenez le parent pour qu'il **recommence** un paiement correct.

## ♻️ Revenir sur une décision
- Il n'y a **pas de corbeille** : on ne « restaure » pas un paiement.
- Pour **annuler une validation** erronée, passez par l'**annulation du paiement** dans
  **Student Fees** (*03*, 🔴) ; le paiement reviendra alors en attente.
- Un paiement **rejeté** peut être **re-validé** plus tard si le parent apporte la preuve,
  en rouvrant la ligne (`fees.ussd-payments.show`) et en validant.

## ⚠️ Bon à savoir
- **Toujours vérifier avant de valider** : valider = garantir que l'argent est là. En cas
  de validation abusive, l'école émet un reçu pour une somme non reçue.
- Le **KPI « À Valider »** est votre file d'attente : traitez-la **chaque jour** pour que
  les reçus des élèves soient à jour.
- La **liste** (`fees.ussd-payments.list`) est **recherchable / exportable**.
- Les **comptes Mobile Money activables** (par opérateur et pays) se gèrent dans les
  **Paramètres** de l'école ; une école « USSD uniquement » n'a pas besoin de FeexPay.
- Les paiements **en ligne par lien/carte (FeexPay)** se suivent dans le **Journal des
  transactions de frais** (*08*), séparé de l'USSD.
