---
id: 04-01-import-intelligent
partie: 4
titre_partie: "Académique : Outils IA"
app: web
slug: 04-01-import-intelligent
emoji: "⚡"
titre: "Import Intelligent Multi-Format (listes d'élèves)"
resume: "Le module le plus puissant pour gagner du temps : vous déposez n'importe quel document contenant une liste d'élèves (Excel, CSV, Word, PDF, photo ou scan d'une liste papier) et l'IA extrait automat..."
audiences: [school_admin]
---
# ⚡ Import Intelligent Multi-Format (listes d'élèves)

## 🎯 Rôle
Le module le plus puissant pour gagner du temps : vous **déposez n'importe quel document**
contenant une liste d'élèves (Excel, CSV, Word, PDF, photo ou scan d'une liste papier) et
l'**IA extrait automatic**ement les noms, prénoms, dates de naissance, classes… puis
**crée les fiches élèves** en un clic après votre validation.

## ✅ Prérequis
1. Avoir créé les **classes** (et sections) qui recevront les élèves.
2. Le fichier/image doit être **lisible** (photo nette, PDF pas protégé).
3. Permission « student-create » + module import inclus dans l'abonnement.
4. Accès : menu **Académique → ⚡ Import Intelligent Multi-Format (NEW)**.

## 🟢 Déroulé complet (étape par étape)
1. Ouvrez le module d'import intelligent.
2. Cliquez sur la zone **Déposer un fichier** (ou glissez-déposez votre document) :
   formats acceptés : Excel (.xlsx/.xls), CSV, Word (.docx), PDF, images (.jpg/.png).
3. Attendez la phase d'**analyse IA** (quelques secondes à 1 minute selon la taille).
4. L'écran affiche un **aperçu tableau** des élèves détectés, colonne par colonne.
5. **Aidez l'IA à bien lire** si besoin : sur chaque colonne détectée, indiquez à quoi
   elle correspond (Nom, Prénom, Sexe, Date de naissance, Classe, Parent, Téléphone…)
   via les listes déroulantes d'en-tête.
6. Corrigez directement dans l'aperçu les lignes mal lues (faute de frappe, date bizarre).
7. Choisissez la **classe de destination** (globale ou par ligne).
8. Vérifiez les **doublons signalés** (l'IA prévient quand un élève semble déjà exister) :
   decidez ligne par ligne — ignorer, fusionner ou importer quand même.
9. Cliquez sur **Importer / Valider l'import**.
10. Un rapport final affiche : « X importés, Y ignorés, Z erreurs ». Les erreurs sont
    téléchargeables pour correction.

## ✏️ Modifier le résultat d'un import
Un import réussi crée des **fiches élèves normales** : elles se corrigent donc
module **Élèves → liste** (crayon ✏️), pas dans l'outil d'import.

## 🔴 Annuler (supprimer) un mauvais import
1. Ouvrez **Élèves → Liste des élèves**.
2. Filtrez par **classe** et par date d'admission (la date d'aujourd'hui) pour isoler
   les élèvesimportés par erreur.
3. Cochez les cases des lignes concernées (ou « tout sélectionner ») → icône
   **poubelle 🗑** pour les envoyer en corbeille en lot.

⚠️ Faites cet « import test » d'abord avec **5 lignes** si vous débutez avec un nouveau format
de document ; une fois que le résultat vous convient, relancez avec le fichier complet.

## ♻️ Restaurer des élèves mal supprimés après import
1. Liste des élèves → filtre **Corbeille / Trashed** (ou « Inactifs » selon l'écran).
2. Sélectionnez les lignes → icône **restaurer ♻️** → confirmez.

## ⚠️ Bon à savoir
- Les **lignes de conseil** du modèle (« remplissez une ligne par élève… ») peuvent être
  lues comme un élève : vérifiez la première ligne de l'aperçu.
- Un fichier **CSV enregistré depuis Excel** doit rester en UTF-8 sinon les accents
  (é, è, ç) s'abîment — préférez .xlsx.
- Les colonnes manquantes (pas de date de naissance sur le document source) ne bloquent
  pas l'import : les champs restent vides et complétables plus tard.
- L'import attibue automatiquement un **mot de passe provisoire** et un matricule si le
  format le prévoit ; utilisez ensuite *Élèves → Réinitialiser mots de passe*.
