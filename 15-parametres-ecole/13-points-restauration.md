---
id: 15-13-points-restauration
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-13-points-restauration
emoji: "🔐"
titre: "Points de restauration (sauvegardes sécurisées) + réinitialisation école"
resume: "Ce module est votre « bouton rembourré » : il crée des points de sauvegarde complets de la base de votre école (payants, sécurisés via FeexPay), permet de revenir en arrière en restaurant un point,..."
audiences: [school_admin]
---
# 🔐 Points de restauration (sauvegardes sécurisées) + réinitialisation école

## 🎯 Rôle
Ce module est votre **« bouton rembourré »** : il crée des **points de sauvegarde complets**
de la base de votre école (payants, sécurisés via FeexPay), permet de **revenir en arrière**
en restaurant un point, et offre une **réinitialisation d'usine** (effacer toute la saisie
pour repartir à zéro — précédée automatiquement d'une **sauvegarde de sécurité téléchargeable**).
À utiliser lors des **grosses opérations** : début d'année, migration de données, nettoyage.

## ✅ Prérequis
1. Être **School Admin**.
2. Avoir un **moyen de paiement** pour les points de sauvegarde (service payant).
3. Accès : **Paramètres → Points de Restauration** (`school-settings.backup-points`).

## 🟢 Créer un point de restauration (étape par étape)
1. Ouvrez **Points de Restauration**.
2. Cliquez **Créer un point** (`school-settings.backup-points.store`) →
   **payez** si demandé (`school-settings.backup.pay`, retour FeexPay
   `backup-points/feexpay/callback/success`).
3. La sauvegarde s'exécute en **tâche de fond** : suivez sa progression
   (`school-settings.backup-points.job-status`) jusqu'à **succès**.
4. Le point apparaît dans la **liste**, daté — nommez-le mentalement
   (« avant rentrée 2026 »).

## ♻️ Restaurer un point (étape par étape)
1. Dans la liste, sélectionnez le **point voulu**.
2. Cliquez **Restaurer** (`school-settings.backup-points.restore`) et **confirmez** :
   l'école repart **exactement** à l'état de ce point.
   ⚠️ Tout ce qui a été saisi **après** le point est **perdu** (sauf la sauvegarde de
   pré-restauration si proposée) — prévenez le personnel **avant**.
3. Attendez la fin de la tâche (bouton d'état), puis **vérifiez** quelques données clés.

## 🧨 Réinitialiser l'école (factory reset)
1. Cas : vous voulez **repartir proprement** (fin de test, re-démarrage d'année).
2. Le système crée **d'abord une sauvegarde de sécurité** que vous pouvez
   **télécharger** (`school-settings.download-pre-reset-backup/{filename}`) —
   **TÉLÉCHARGEZ-LA ET GARDEZ-LA**.
3. Confirmez la **réinitialisation** (`school-settings.factory-reset`) : les données
   d'exploitation sont effacées, l'école reste active.
4. Pour revenir en arrière plus tard : **restaurer** un point ou demander la réinjection du
   fichier au Support EduEasy.

## ✏️ Modifier / 🔴 Supprimer
- Les points **se consultent** ; leur **suppression/conservation** suit la politique de
  rétention de la plateforme (les anciens points restent la seule « version » dispo).

## ⚠️ Bon à savoir
- **Rythme conseillé** : 1 point **avant chaque grande vague** de saisie (rentrée, promotion,
  import de masse).
- **Restauration = voyage dans le temps** : prévenez **toute la caisse** — un paiement saisi
  après le point **disparaît** avec la restauration.
- **Sauvegarde ≠ abonnement** : ce module protège vos **données** ; l'abonnement se gère en
  *15*.
- La **sauvegarde .sql manuelle** (téléchargement libre) existe aussi :
  *14-sauvegarde-base.md*.
- En cas de **doute avant restauration**, appelez d'abord le **Support EduEasy**.
