---
id: 09-12-questions-examens-en-ligne
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-12-questions-examens-en-ligne
emoji: "❓"
titre: "Gérer et importer les questions d'examens en ligne (QCM)"
resume: "Les questions sont la matière première des examens en ligne : énoncé + plusieurs choix de réponse (QCM) + bonne(s) réponse(s) + difficulté."
audiences: [school_admin]
---
# ❓ Gérer et importer les questions d'examens en ligne (QCM)

## 🎯 Rôle
Les **questions** sont la matière première des **examens en ligne** : énoncé + **plusieurs
choix de réponse** (QCM) + **bonne(s) réponse(s)** + **difficulté**. Cette page explique
comment **créer une question à la main**, en **ajouter plusieurs d'un coup via un fichier
CSV**, et comment **tirer des questions aléatoirement par niveau de difficulté** pour composer
un examen. Les questions sont rangées par **classe/section + matière**, prêtes à être
attachées à un examen en ligne (*11*).

## ✅ Prérequis
1. Permission « online-exam-create ».
2. Avoir **classes / sections / matières**.
3. Accès : menu **Online Exam → Gérer les questions** (`online-exam-question.index`) et
   **Ajouter des questions en masse** (`online-exam-question.add-bulk-questions`).

## 🟢 Créer une question manuellement (étape par étape)
1. Ouvrez **Gérer les questions**, puis l'examen / la section concernée pour arriver sur la
   page **« Assigner les questions »** (sous-titre : *« Ajoutez des questions manuellement ou
   tirez-les aléatoirement par difficulté. »*).
2. Choisissez le mode **« manuel »** et remplissez :
   - **Class Section** et **Sujet / Matière** (souvent pré-remplis selon l'examen) ;
   - **« question »** ★ — l'énoncé (zone de texte, format riche possible) ;
   - les **options** de réponse : « option 0 », « option 1 »… Cliquez **« add_option »** pour
     **ajouter une ligne de choix** (✕ pour en retirer une) ;
   - **« answer »** ★ — la/les **bonne(s) réponse(s)** : sélectionnez dans la liste les
     options correctes (multi-choix) ;
   - **Image** (facultatif) — illustration de la question ;
   - **Note** — libellé/consigne éventuelle ;
   - **« difficulty »** ★ — **easy / medium / hard** (Facile / Moyen / Difficile).
3. **Enregistrez / Submit**. La question rejoint la **banque de questions** de cette
   classe/matière.

## 🎲 Tirer des questions au hasard (par difficulté)
1. Sur la même page, choisissez le mode **« random »** (questions aléatoires).
2. Indiquez la **difficulté** souhaitée (easy/medium/hard) et le **nombre** de questions à
   tirer.
3. Validez (`store-random-choice-question`) : le logiciel **sélectionne automatiquement** des
   questions de la banque selon la difficulté demandée et les attache à l'examen.

## 📥 Ajouter des questions en masse (CSV)
1. Ouvrez **Online Exam → Ajouter des questions en masse** (sous-titre : *« Importez
   plusieurs questions d'un coup via un fichier CSV. »*).
2. Sélectionnez :
   - **Class Section** ★ (multi-choix, « Select All » possible) ;
   - **subject** ★ (la matière).
3. **Téléchargez le fichier modèle**, **remplissez-le** (énoncé, options, bonne réponse,
   difficulté) puis **enregistrez en .CSV**.
4. **Téléversez** le fichier et **Soumettez** : toutes les questions sont **créées d'un coup**.

## ✏️ Modifier / 🔴 Supprimer une question
- Depuis **Gérer les questions** (liste des questions d'une classe/matière), chaque ligne
  propose l'**édition** (corriger énoncé, options, bonne réponse, difficulté) et la
  **suppression**.
- ⚠️ Une question **déjà utilisée dans un examen passé** : la modifier n'efface pas les copies
  déjà rendues ; corrigez plutôt **avant** de lancer l'examen.

## ♻️ Restaurer
- Les questions supprimées **ne disposent pas de corbeille restaurable** : si effacées par
  erreur, **recréez-les** (à la main ou par import CSV). Conservez une copie de vos fichiers
  de questions.

## ⚠️ Bon à savoir
- **Bien marquer la bonne réponse** : la correction automatique de l'examen en ligne dépend
  entièrement de la/les option(s) sélectionnée(s) dans **« answer »**.
- **Équilibrez les difficultés** (easy/medium/hard) pour un examen juste : le tirage aléatoire
  s'appuie sur ce champ.
- Une question appartient à **une classe/section + une matière** : rangez-les au bon endroit,
  sinon elles n'apparaîtront pas au moment d'assigner l'examen.
- **Format .CSV obligatoire** pour l'import en masse ; ne changez pas les colonnes du modèle.
- Pour assembler ces questions dans un examen, voyez *11-examens-en-ligne.md*.
