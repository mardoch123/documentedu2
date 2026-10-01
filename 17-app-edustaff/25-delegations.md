---
id: 17-25-delegations
partie: 17
titre_partie: "Application EduStaff"
app: edustaff
slug: 17-25-delegations
emoji: "🤝"
titre: "déléguer des permissions et en demander"
resume: "Le compte School Admin peut prêter des droits précis à un membre du personnel — encaisser à la place, valider l'USSD, configurer les paiements — pour une durée limitée ou permanente, sans partager ..."
audiences: [teacher, staff, school_admin]
---
# 🤝 17.25 — EduStaff : déléguer des permissions et en demander

## 🎯 Rôle
Le **compte School Admin** peut prêter des droits précis à un membre du personnel —
encaisser à la place, valider l'USSD, configurer les paiements — **pour une durée
limitée ou permanente**, sans partager le mot de passe. Le salarié, lui, peut
**demander** une permission depuis son app.

## ✅ Prérequis
1. Être **School Admin** pour accorder ; tout membre du personnel pour demander.
2. La personne visée doit avoir un compte actif (page 17.19).

## 🟢 Accorder une délégation (étape par étape)
1. Accueil direction → **« + »** → famille **Gestion du personnel** (ou Outils) →
   **« Accorder une permission »** (écran « Accorder la permission de paiement »).
2. **Sélectionnez le membre du staff** concerné dans la liste.
3. Choisissez le **type de permission** :
   - **Réception de paiements** (encaisser à la caisse, page 17.20) ;
   - **Validation USSD** (valider les paiements parent, pages 17.20–17.21) ;
   - **Configuration des moyens de paiement** (le hub page 17.21) ;
   - autres types définis par l'école.
4. Fixez la **durée** : limitée (avec date de fin) ou **permanente**.
5. **Confirmer** : l'intéressé reçoit la permission dès son écran suivant — les tuiles
   cachées deviennent visibles.
6. L'écran **« Délégations »** liste toutes les permissions en cours, avec qui, quoi,
   jusqu'à quand.

## 🟢 Demander une permission (salarié)
1. Tuile **« Demander une permission »**.
2. Choisissez le droit souhaité, la **durée** et le **motif**.
3. **Envoyer** : la direction voit la demande dans **« Demandes de permission »**
   (avec badge 🔔 sur l'accueil) et l'**approuve ou refuse**.

## ✏️ Modifier / révoquer
1. Écran **« Délégations »** → ouvrez la ligne.
2. Changer **durée/type** : révocation puis nouvelle accord (plus clair que de
   glisser une date sans trace).
3. **Révoquer** immédiatement : le membre perd la tuile dès la prochaine ouverture
   d'écran — les actes déjà faits sous délégation restent valables et journalisés.

## 🔴 Supprimer une délégation
- C'est la **révocation** ci-dessus : supprimer la ligne ne se fait pas, on **retire
  le droit** — l'historique de la délégation reste consultable.

## ♻️ Restaurer
- Permission retirée par erreur : **accordez-la de nouveau** (2 minutes, même écran).
- Délégation expirée dont on a encore besoin : re-créez-la avec une durée plus
  longue — évitez le renouvellement tacite de permanences.
- Le délégué dit ne pas voir la tuile : **déconnectez-reconnectez** son compte, ou
  vérifiez qu'une autre délégation du même type ne lui a pas été révoquée entre-temps.

## ⚠️ Bon à savoir
- **Délégation ≠ compte admin** : le délégué n'a que le droit prêté, pas la gestion
  du personnel ni les paramètres.
- Privilégiez les durées **limitées** (remplacement de congé = la durée exacte du
  congé) : moins de risque, piste d'audit plus claire.
- Chaque encaissement sous délégation porte le **nom du réel exécutant** sur le reçu
  et dans les logs — la responsabilité reste nominale.
- La permission **« configuration des paiements »** ne se donne qu'à une personne de
  confiance : son titulaire peut changer les clés FeexPay et les comptes USSD.
