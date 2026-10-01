---
id: 10-03-paiements-eleves
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-03-paiements-eleves
emoji: "💶"
titre: "Encaisser et suivre les paiements des élèves (Student Fees)"
resume: "C'est le guichet de l'école : là où l'on encaisse ce que les familles règlent (espèces, mobile money, etc.), édite un reçu et suit qui a payé, combien, et ce qui reste à payer."
audiences: [school_admin, staff]
---
# 💶 Encaisser et suivre les paiements des élèves (Student Fees)

## 🎯 Rôle
C'est le **guichet de l'école** : là où l'on **encaisse** ce que les familles règlent
(espèces, mobile money, etc.), **édite un reçu** et **suit** qui a payé, combien, et ce qui
**reste à payer**. Cette page couvre la **liste des frais par élève**, l'**encaissement**,
le **reçu imprimable** et la **correction/suppression** d'un paiement.

## ✅ Prérequis
1. Avoir **créé une grille de frais** (*02*) : sans grille, aucun montant dû n'existe.
2. Permission « fees-paid ».
3. Accès : menu **Fees → Student Fees** (`fees.paid.index`) — page **« Frais encaissés »**.

## 🟢 Encaisser un paiement (étape par étape)
1. Ouvrez **Student Fees / Frais encaissés** (sous-titre : *« Suivez et gérez tous les
   paiements encaissés, les tranches et les journaux de caisse. »*).
2. **Filtrez** pour retrouver l'élève : **Année scolaire**, **Frais par classe**,
   **Class Section**, **Statut** (payé / partiel), filtre **hebdomadaire** ou **semaine**
   personnalisée, et statut de **reste à payer** (« Reste à payer (> 0) »,
   « Non payée (0 FCFA versé) »).
3. Sur la ligne de l'élève, lancez l'**encaissement** (bouton Payer / page de paiement
   `pay-compulsory`) :
   - consultez le **« Détail des rubriques & Tranches »** (ce qui est dû, ce qui reste) ;
   - saisissez le **montant** reçu, le **mode de paiement**, éventuellement une
     **référence de transaction** ;
   - validez : le paiement est **enregistré** et le **reste à payer diminue**.
4. Le **total encaissé** et le **nombre de paiements de la semaine** se mettent à jour.

## 🧾 Éditer / imprimer un reçu
- Chaque paiement donne un **reçu** (`fees.paid.receipt.pdf`) : **PDF imprimable** ou
  **reçu thermique 58 mm** (petite caisse) via la fenêtre d'impression thermique.
- Les **parents** peuvent aussi retrouver leurs reçus dans leur espace / par lien de
  vérification.

## ✏️ Corriger un paiement
1. Sur le paiement concerné, utilisez l'**action Modifier** (mise à jour du **montant**
   encaissé via « update-amount », ou édition de la ligne payée).
2. **Enregistrez** : le montant et le reste à payer sont recalculés.

## 🔴 Supprimer / annuler un paiement
Sur la fiche de l'élève, selon la nature du paiement :
- **« remove-optional-fee »** : retirer un **frais optionnel** payé à tort ;
- **« remove-installment-fees »** : retirer une **tranche** payée à tort ;
- **« remove-all-installment-payments »** : annuler **tous les versements** d'une tranche
  pour cet élève et ce frais.
> ⚠️ Une **suppression de paiement** n'est **pas restaurable** par corbeille : le paiement
> effacé doit être **ré-encaissé** manuellement si c'était une erreur.

## ♻️ Restaurer un paiement supprimé
- Il n'y a **pas de corbeille pour les encaissements** : pour « revenir » sur un paiement
  supprimé, **encaissez à nouveau** le bon montant.
- Le **Journal des transactions** (*08-journal-transactions-frais.md*) garde l'**historique**
  des opérations en ligne (réussies / en attente / échouées) pour tracer un doute.

## 🔁 Transférer un paiement entre enfants d'un même parent
- L'action **Transfert de paiement** (`fees.transfer.index`) permet de **réaffecter un paiement**
  d'un élève vers **un autre élève du même parent/tuteur** (ex. un trop-perçu sur l'aîné remis
  au cadet) : recherchez l'élève, vérifiez les détails, validez le transfert.

## ⚠️ Bon à savoir
- **Paiement séquentiel** : si activé dans Fees Config, les tranches doivent être payées
  **dans l'ordre** (on ne saute pas une tranche).
- **Reste à payer = 0** → l'élève apparaît **« payé »** ; au-delà des échéances → **impayé**
  (peut déclencher les **renvois**).
- Le **reçu 58 mm** est idéal pour la caisse physique ; le **PDF** pour l'envoi au parent.
- Les **paiements USSD / mobile money** initiés par les parents passent d'abord en
  **validation** par la direction (*07-paiements-ussd.md*) avant de créditer l'élève.
