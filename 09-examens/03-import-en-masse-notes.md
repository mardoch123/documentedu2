---
id: 09-03-import-en-masse-notes
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-03-import-en-masse-notes
emoji: "📥"
titre: "Importer les notes en masse (fichier CSV / Excel)"
resume: "Quand une classe compte beaucoup d'élèves ou plusieurs matières, saisir note par note est long."
audiences: [school_admin, teacher]
---
# 📥 Importer les notes en masse (fichier CSV / Excel)

## 🎯 Rôle
Quand une classe compte beaucoup d'élèves ou plusieurs matières, **saisir note par note est
long**. L'**import en masse** permet de remplir les notes depuis un **fichier tableur**
(CSV), en une seule opération : on **télécharge le modèle**, on le **remplit dans Excel**,
puis on le **renvoie**.

## ✅ Prérequis
1. Avoir **créé l'examen** et la **matière** correspondante (*01*, *04*).
2. Permission « exam-upload-marks ».
3. Un fichier **CSV** prêt (généré depuis le modèle fourni, voir étapes).
4. Accès : menu **Offline Exam → Import en masse des notes** (`exam.bulk-upload-marks`).

## 🟢 Importer les notes (étape par étape)
1. Ouvrez **Importer les notes en masse**.
2. Sélectionnez les trois filtres enchaînés :
   - **Classe / Section** ★ ;
   - **Examen** ★ (se remplit selon la classe) ;
   - **Matière** ★ (sélecteur multi-choix).
3. Cliquez **« Télécharger le fichier modèle »** (*download dummy file*).
4. ⚠️ **Le modèle se télécharge d'abord** : **ouvrez-le dans Excel**, **remplissez la colonne
   des notes** pour chaque élève (en respectant les N° d'élève / matricules déjà listés),
   puis **enregistrez-le au format .CSV**.
   > Note affichée : *« First download dummy file and convert to .csv file then upload it »* —
   > il faut donc **d'abord télécharger, remplir, convertir en .csv, puis téléverser**.
5. Dans la zone **« file_upload »** ★, cliquez **« upload »** et choisissez votre fichier
   **.csv** rempli.
6. Cliquez **« submit »**.
7. Les notes sont **importées pour tous les élèves d'un coup** et le tableau se rafraîchit.

## ✏️ Corriger une note importée par erreur
- Relancez simplement l'**import avec le fichier corrigé** pour la même classe/examen/matière :
  l'import **met à jour** les notes existantes (il ne crée pas de doublon).
- Ou corrigez la ou les valeurs à la main dans **Saisir les notes** (*02*).

## 🔴 Annuler un import
- Il n'existe **pas de « dé-import » ni de corbeille** pour les notes importées.
- Pour « retirer » des notes importées à tort, **re-importez un fichier** où ces notes sont
  remises à **0** (ou videz et re-soumettez la saisie manuelle).

## ♻️ Restaurer après un mauvais import
- La dernière importation **écrase** la précédente : pour revenir en arrière, **re-importez le
  bon fichier**. Conservez toujours **une copie de secours** de vos fichiers CSV importés.

## ⚠️ Bon à savoir
- **Ne modifiez pas la structure du modèle** (colonnes, ordre, identifiants d'élèves) : seul
  le **contenu des notes** doit être modifié. Un fichier mal formaté est rejeté.
- **Format .CSV obligatoire** à l'envoi (Excel peut « Enregistrer sous → CSV »).
- Faites l'import **matière par matière** si le modèle est organisé ainsi : vérifiez que la
  bonne matière est sélectionnée avant d'envoyer.
- Après import, **consultez les notes non publiées** (*05*) pour contrôler avant de publier.
- Pour une seule note à changer, la **saisie manuelle** (*02*) est plus rapide que de refaire
  tout un import.
