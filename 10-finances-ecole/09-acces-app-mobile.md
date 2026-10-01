---
id: 10-09-acces-app-mobile
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-09-acces-app-mobile
emoji: "📲"
titre: "Vendre / renouveler les accès à l'application mobile"
resume: "Les applications mobiles (EduStudent pour l'élève/parent, EduStaff pour le personnel) fonctionnent par abonnement."
audiences: [school_admin, staff]
---
# 📲 Vendre / renouveler les accès à l'application mobile

## 🎯 Rôle
Les **applications mobiles** (EduStudent pour l'élève/parent, EduStaff pour le personnel)
fonctionnent par **abonnement**. Cette page (**Accès App Mobile**) permet à l'école de
**vendre, renouveler et contrôler l'accès** de chaque apprenant à son application : voir qui
a un **accès actif** ou **verrouillé**, connaître la **formule** souscrite et le **dernier
règlement**, et **abonner manuellement** un élève. ⚠️ Réservé au **School Admin**.

## ✅ Prérequis
1. Être **School Admin** (gestionnaire de l'école) — cette page ne s'ouvre pas aux autres
   rôles.
2. Option « **Fees Management** » + permission associée.
3. Accès : menu **Fees → Accès App Mobile** (`fees.app-subscriptions.index`).

## 📋 Consulter les accès (étape par étape)
1. Ouvrez **Accès App Mobile** (titre : *« Abonnements & Accès App Mobile »*).
2. Consultez les **KPI** : **« Accès Actifs »** et **« Accès Verrouillés »** (combien
   d'élèves peuvent ou non utiliser l'app).
3. Dans **« Liste Apprenants »**, **filtrez par Classe** pour cibler un groupe.
4. Lisez le tableau : colonnes **Matricule, Apprenant, Classe, Statut (actif/verrouillé),
   Formule, Dernier Règlement, Action**.

## 🟢 Abonner / renouveler manuellement un accès
1. Sur la ligne de l'élève, cliquez l'action d'**abonnement manuel**
   (`fees.app-subscriptions.manual-subscribe`).
2. Choisissez la **formule / durée** de l'abonnement.
3. Validez : l'élève passe en **accès actif**, il peut ouvrir et utiliser l'application.
4. (La liste des abonnements se recharge via `fees.app-subscriptions.list`.)

## 🔴 Verrouiller / laisser expirer un accès
- Un accès **non renouvelé** ou annulé repasse en **« Verrouillé »** : l'élève n'a plus
  accès à l'app (mais reste élève de l'école).
- Le **verrouillage** se fait par l'action correspondante sur la ligne (changement de
  statut).

## ♻️ Rétablir un accès coupé
- Pas de corbeille : pour **rétablir** un accès verrouillé, il suffit de le
  **ré-abonner manuellement** (`manual-subscribe`) — l'accès redevient **actif**.

## ⚠️ Bon à savoir
- **Accès ≠ scolarité** : l'abonnement à l'app mobile est un **service payant distinct**
  des frais scolaires ; il se renouvelle sur sa propre **formule/durée**.
- Le **« Dernier Règlement »** indique la date à vérifier pour le **prochain renouvellement**.
- **Filtrer par classe** aide à faire des **campagnes de renouvellement** (ex. relancer
  toutes les 6èmes dont l'accès expire).
- Si un parent **ne peut pas se connecter** à l'app, vérifiez d'abord ici le **Statut** :
  « Verrouillé » = problème d'abonnement, pas de mot de passe.
- La **config des moyens de paiement** (FeexPay, KKiaPay, USSD, espèces) pour ces ventes se
  fait dans les **Paramètres → Moyens de paiement** de l'école.
