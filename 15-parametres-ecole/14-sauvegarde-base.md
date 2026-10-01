---
id: 15-14-sauvegarde-base
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-14-sauvegarde-base
emoji: "💾"
titre: "Sauvegarde de la base de données (télécharger / restaurer un .sql)"
resume: "Cette page donne à l'école un accès direct et autonome à ses sauvegardes SQL : créer une sauvegarde de la base de l'école, la télécharger en fichier .sql (à garder sur une clé US"
audiences: [school_admin]
---
# 💾 Sauvegarde de la base de données (télécharger / restaurer un .sql)

## 🎯 Rôle
Cette page donne à l'école un accès **direct et autonome** à ses **sauvegardes SQL** : créer
une sauvegarde de la base de l'école, la **télécharger** en fichier `.sql` (à garder sur une
clé USB — la vraie assurance tous risques), la **restaurer** si besoin, et **supprimer** les
fichiers de sauvegarde devenus inutiles.

## ✅ Prérequis
1. Être **School Admin**.
2. Comprendre qu'un fichier `.sql` est une **copie complète des données** — il est
   **sensible** (notes, paiements, contacts) : **ne jamais le partager publiquement**.
3. Accès : **Paramètres → Database Backup** (`database-backup.index`).

## 🟢 Créer une sauvegarde (étape par étape)
1. Ouvrez **Database Backup**.
2. Cliquez **Générer / Créer la sauvegarde** (`database-backup.store`) : le fichier `.sql`
   est produit et apparaît dans la **liste** (`database-backup.show`).
3. **Téléchargez-le** immédiatement (`database-backup.download/{filename}`) et rangez-le :
   `C:/Ecole/Sauvegardes/2026-09-30.sql` (date dans le nom !).

## ♻️ Restaurer une sauvegarde
1. Dans la liste des fichiers présents sur le serveur, choisissez la sauvegarde.
2. Cliquez **Restaurer** (`database-backup.restore/{id}`) et **confirmez** : les données
   reviennent à l'état du fichier.
   ⚠️ Comme toute restauration : ce qui a été saisi **après** est écrasé. Prévenez la caisse
   et le secrétariat.
3. **Contrôlez** après restauration : solde d'un élève, dernier paiement, liste de classe.

## 🔴 Supprimer un fichier de sauvegarde
1. Depuis la liste serveur : **supprimer le fichier** (`database-backup.destroy-file` /
   `database-backup.destroy/{id}`).
2. ⚠️ La suppression est **définitive** : ne supprimez **jamais la dernière copie** d'une
   période contenant des paiements.

## ♻️ (après suppression)
- Un fichier `.sql` **supprimé du serveur** peut être **réinjecté** si vous avez gardé le
  **téléchargement local** : demandez sa réinjection au Support EduEasy. **C'est pour cela
  qu'on télécharge toujours après création.**

## ⚠️ Bon à savoir
- **Rythme simple** : 1 sauvegarde **téléchargée** à chaque **fin de mois** + 1 **avant**
  toute grosse opération (voir *13* pour la version professionnelle avec points de
  restauration).
- **Fichier = preuve** : en cas de litige de paiement ancien, la sauvegarde du mois
  concerné **retrouve** l'information même si l'écran a changé depuis.
- **Ne modifiez jamais** un `.sql` avec Word/Excel : c'est un fichier machine ;
  restaurer un fichier **édité** peut échouer.
- **Règle des deux copies** : clé USB **et** un second emplacement (autre PC ou disque cloud).
- La page *13* (points de restauration) est **payante mais pilotée** (tâches, états,
  sécurité) ; ici vous êtes **seul maître** du fichier — responsabilisé mais gratuit.
