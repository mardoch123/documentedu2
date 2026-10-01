---
id: 17-20-encaissement-frais
partie: 17
titre_partie: "Application EduStaff"
app: edustaff
slug: 17-20-encaissement-frais
emoji: "💰"
titre: "EduStaff (caisse) : encaisser les frais scolaires et imprimer les reçus"
resume: "Au guichet de l'école, encaisser un paiement d'élève (espèces, mobile money, USSD) dans l'application, imprimer le reçu thermique, et relancer les parents impayés par WhatsApp ou"
audiences: [teacher, staff, school_admin]
---
# 💰 17.20 — EduStaff (caisse) : encaisser les frais scolaires et imprimer les reçus

## 🎯 Rôle
Au guichet de l'école, **encaisser un paiement d'élève** (espèces, mobile money,
USSD) dans l'application, imprimer le **reçu thermique**, et **relancer les parents**
impayés par WhatsApp ou SMS — l'équivalent mobile de la caisse web (PARTIE 10).

## ✅ Prérequis
1. Être School Admin ou caissier habilité (délégation « payment_reception »,
   page 17.25).
2. Que les **frais et échéances** existent (créés sur le web, PARTIE 10).
3. Pour l'impression : une **imprimante thermique 58 mm** appairée au téléphone
   (écran « Imprimante thermique »).

## 🟢 Encaisser un frais (étape par étape)
1. Accueil → **« + »** → famille **Encaissement & Paiements** → **« Encaisser un frais »**
   (ou lancez depuis la fiche de l'élève).
2. Recherchez l'**élève** (nom ou matricule) : l'écran de paiement s'ouvre avec son
   nom **pré-rempli**.
3. La liste des **frais dus** apparaît : libellé, échéance, **montant dû**.
   ⚠️ Si l'élève a une **réduction active**, un bandeau l'affiche avec le **montant
   net après réduction** — encaissez le net, pas le brut.
4. Touchez le frais à encaisser puis le bouton **« Encaisser »**.
5. Choisissez le **mode** : espèces (saisie du montant reçu) ou mobile money/FeexPay.
6. Validez : message de succès, le reçu est proposé — bouton **« Imprimer le reçu »**
   (format 58 mm) ou partage PDF.
7. Pour encaisser **plusieurs frais d'affilée** : bouton **« Suivant — Encaisser un
   Frais »** qui enchaîne sans re-chercher l'élève.

## 🟢 Valider un paiement USSD parent
1. Même famille → **« Paiements USSD (validation) »** — le badge 🔔 de l'accueil
   signale les en attente.
2. La liste des transactions USSD reçues (montant, référence, opérateur).
3. Ouvrez une ligne : détails de l'élève et du frais concerné.
4. **Approuvez** (« Oui, valider ») pour imputer le paiement, ou refusez avec motif.
5. Une fois par frais, la mention de la **réduction appliquée** s'imprime sur le reçu.

## 🟢 Relancer un parent impayé
1. Fiche **détail des frais de l'élève** → bouton **Relancer / Partager**.
2. Choisissez le canal : **« Partager via WhatsApp »** (message pré-formaté prêt à
   envoyer), **« Envoyer par SMS »**, ou **« Copier le message »**.
3. Le message reprend l'élève, le frais, le montant dû et l'échéance.

## 🟢 Voir les paiements passés
- **« Paiements des élèves »** : historique par élève (qui a payé quoi, quand, combien).
- **« Frais payés »** : toutes les encaissements de la période, filtrable — la
  comptabilité du jour.
- **« Transfert de paiement »** : basculer un trop-perçu d'un frais sur un autre.

## ✏️ Modifier / annuler un encaissement
1. Liste des paiements de l'élève → ouvrez la ligne erronée.
2. **Annuler le paiement** (selon droits) : le frais redevient dû, le reçu est marqué
   annulé — l'opération est journalisée.
3. Un encaissement **ne se réédite pas** avec un autre montant : annulez puis
   ré-encaissez.

## 🔴 Supprimer
- Les encaissements **ne se suppriment jamais** (obligation comptable) : on annule,
  on ne détruit pas. L'écran « Configurer sur le Web » guide vers le web pour les
  cas rares (erreur de session).

## ♻️ Restaurer
- Reçu perdu/réimprimable : liste des paiements → la ligne → **« Imprimer le reçu »**
  encore disponible.
- Paiement USSD payé mais pas dans la liste : le parent doit donner la **référence**
  exacte du SMS opérateur ; vérifiez aussi les filtres de date.
- Annulation faite par erreur : ré-encaissez le même montant, le solde de l'élève
  revient identique.

## ⚠️ Bon à savoir
- **Toujours encaisser le montant net affiché** après réduction : le brut prêterait à
  contestation (le reçu, lui, mentionne la réduction).
- L'imprimante 58 mm doit être **choisie dans l'écran Imprimante thermique** avant le
  premier reçu de la journée.
- Un double encaissement (parent qui paie deux fois) se **corrige par transfert** ou
  remboursement déclaré dans « Paiements des élèves » — jamais par effacement.
- La caisse de l'application **n'imprime pas les reçus A4** officiels : ceux du web
  (PARTIE 10) restent la référence pour les familles qui les exigent.
- Besoin de créer un nouveau type de frais ? Ça se passe sur le web (PARTIE 10,
  « Ajouter des frais ») — l'app ne fait qu'encaisser l'existant.
