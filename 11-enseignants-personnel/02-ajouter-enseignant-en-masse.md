---
id: 11-02-ajouter-enseignant-en-masse
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-02-ajouter-enseignant-en-masse
emoji: "📥"
titre: "Import en masse des enseignants"
resume: "Plutôt que d'inscrire les enseignants un par un, l'import en masse (Bulk Upload) permet de créer des dizaines de fiches d'un coup à partir d'un fichier Excel/CSV préparé à l'avance."
audiences: [school_admin]
---
# 📥 Import en masse des enseignants

## 🎯 Rôle
Plutôt que d'inscrire les enseignants **un par un**, l'**import en masse (Bulk Upload)**
permet de créer **des dizaines de fiches d'un coup** à partir d'un **fichier Excel/CSV**
préparé à l'avance. Gain de temps précieux en **rentrée scolaire** ou lors d'une grande
campagne de recrutement.

## ✅ Prérequis
1. Permission « **teacher-create** » (ou teacher-edit).
2. Un fichier **CSV** au **format attendu** (téléchargeable via le modèle).
3. Accès : menu **Teacher → Bulk upload** (`teachers.create-bulk-upload`).

## 🟢 Importer des enseignants (étape par étape)
1. Ouvrez **Bulk upload** ( enseignants).
2. **Téléchargez le modèle** (fichier d'exemple) : bouton du **dummy/sample file**
   (`teachers.bulk-data-sample`) — il donne les **colonnes exactes** à remplir.
3. **Remplissez le fichier** avec vos enseignants : une ligne = un enseignant (prénom, nom,
   sexe, email **unique**, mobile, date de naissance, qualification, adresses, type de
   paiement, salaire/taux horaire…).
4. **Reprenez le fichier** dans la zone d'envoi (format **.csv / .txt** accepté).
5. Cochez ou non l'option **« envoyer une notification »** (`is_send_notification`) : si
   activée, chaque enseignant créé reçoit un **email/compte**.
6. Cliquez **« Importer »** (`teachers.store-bulk-upload`). Message :
   « **Données enregistrées avec succès.** »
7. Les enseignants apparaissent dans **Manage Teacher** (*01*).

## ✏️ Corriger après import
- Un import ne se « modifie » pas en bloc : corrigez **chaque fiche** dans *Manage Teacher*
  (*01*, ✏️).
- Si des lignes ont été **refusées** (email dupliqué, champ manquant), **corrigez le
  fichier** et **réimportez uniquement** les lignes manquantes.

## 🔴 Annuler un import raté
- Il n'y a **pas de bouton « annuler l'import »** : repérez les enseignants créés par erreur
  dans la liste et **supprimez-les** (corbeille) ou **désactivez-les** — voir *03*.
- Pour éviter les doublons, **ne relancez pas** un import déjà réussi : l'**email unique**
  bloquera les lignes déjà présentes (mais créera quand même les nouvelles).

## ♻️ Restaurer
- Les enseignants importés puis **supprimés** se **restaurent** normalement via l'onglet
  **« Trashed »** + **Restaurer** (voir *03-supprimer-restaurer-enseignant.md*).

## ⚠️ Bon à savoir
- **Respectez l'entête du modèle** : les colonnes doivent être **nommées et ordonnées**
  exactement comme le fichier d'exemple, sinon l'import échoue.
- **Email unique obligatoire** : une ligne avec un email **déjà existant** sera **refusée**.
- **Mobile** : 6 à 15 chiffres, sans lettres.
- **Séparateur** : enregistrez le CSV en **UTF-8** pour éviter les accents cassés.
- Faites un **essai avec 2-3 lignes** d'abord, vérifiez, puis importez le gros fichier.
- Le même principe d'import existe pour le **personnel non enseignant** (*04*) et les
  **élèves** (voir PARTIE Élèves).
