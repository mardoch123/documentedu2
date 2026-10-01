---
id: 09-02-saisir-notes-examen
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-02-saisir-notes-examen
emoji: "⌨️"
titre: "Saisir les notes d'un examen (manuel, dictée vocale, scan OCR)"
resume: "Après avoir créé l'examen et son emploi du temps, l'enseignant (ou la direction) entre les notes de chaque élève, matière par matière."
audiences: [school_admin, teacher]
---
# ⌨️ Saisir les notes d'un examen (manuel, dictée vocale, scan OCR)

## 🎯 Rôle
Après avoir créé l'examen et son emploi du temps, l'enseignant (ou la direction) **entre les
notes de chaque élève, matière par matière**. Cette saisie peut se faire **au clavier**, ou
grâce à deux aides **IA** très utiles pour les non-technophiles : la **dictée vocale** (on
dicte les notes à voix haute) et le **scan OCR** (on photographie la feuille de notes et le
logiciel la lit tout seul).

## ✅ Prérequis
1. Avoir **créé l'examen** (*01*) et son **emploi du temps / matière** (*04*).
2. Permission « exam-upload-marks ». Un **enseignant** ne voit que ses classes/matières.
3. Être connecté (le prof concerné ou la direction).
4. Accès : menu **Offline Exam → Saisir/notes d'examen** (`exams.upload-marks`).

## 🟢 Saisir les notes au clavier (étape par étape)
1. Ouvrez **Saisir les notes d'examen**. Le bloc **« Créer les notes »** est en haut.
2. Choisissez les trois filtres obligatoires enchaînés :
   - **Classe / Section** ★ →
   - **Examen** ★ (la liste se remplit selon la classe choisie) →
   - **Matière** ★ (matières de la classe pour cet examen).
3. La **liste des élèves** de cette classe/matière s'affiche dans un tableau, avec pour
   chacun une case de **note obtenue** (et le **barème / total** de la matière).
4. Tapez la note de chaque élève dans sa case.
5. Cliquez **« submit »** pour **enregistrer toutes les notes** d'un coup.
   > Enregistrer une 2ᵉ fois la même classe/examen/matière **met à jour** les notes déjà
   > saisies (pas de doublon).

## 🎙️ Dictée Vocale IA (gagner du temps)
1. Au-dessus du tableau, cliquez **« 🎙️ Dictée Vocale IA »**.
2. Autorisez le **micro**, dictez les notes élève par élève selon les consignes affichées.
3. Les notes reconnues se placent automatiquement dans les cases ; **vérifiez** puis
   **Soumettre**.

## 📸 Scanner une feuille de notes (OCR IA)
1. Cliquez **« 📸 Scanner Feuille OCR (IA) »**.
2. **Prenez en photo** ou téléversez l'image de votre **feuille de notes manuscrite/imprimée**.
3. Le logiciel **extrait les notes** et les pré-remplit dans le tableau.
4. **Contrôlez** chaque valeur (l'OCR peut se tromper sur un chiffre mal écrit), corrigez si
   besoin, puis **Soumettre**.

## ✏️ Modifier une note déjà saisie
1. Revenez sur **Saisir les notes**, reprenez la **même classe / examen / matière**.
2. Les notes existantes se rechargent ; changez la case de l'élève concerné.
3. **Soumettre** — la nouvelle valeur remplace l'ancienne.

## 🔴 « Supprimer » une note / un relevé
- Il n'y a **pas de corbeille pour les notes individuelles** : pour « retirer » une note,
  **remettez-la à 0** ou videz la case et **Soumettez** (la saisie est un système de
  mise à jour : la dernière soumission gagne).
- Pour annuler **tout un examen**, supprimez l'examen lui-même (*01*), mais seulement tant
  qu'aucune note n'est validée/publiée.

## ♻️ Restaurer des notes écrasées
- **Pas d'historique des notes** : si vous écrasez une bonne note, il faut la **re-saisir**.
- Astuce : gardez votre **cahier de notes** ou un **tableur** en parallèle ; en cas d'erreur,
  vous pouvez **repointer** la valeur exacte, ou ré-importer via le fichier CSV
  (*03-import-en-masse-notes.md*).

## ⚠️ Bon à savoir
- **Resélectionnez toujours la même matière** : une note est liée à classe + examen + matière.
  Changer de matière = un autre relevé.
- Le **barème** (note max) vient de la matière/emploi du temps ; saisissez des notes **≤ au
  total**.
- Les notes **ne sont visibles des familles qu'après publication** de l'examen
  (*06-publier-resultats.md*). Avant, elles sont « non publiées » (voir *05*).
- Après une **dictée vocale** ou un **scan OCR**, la relecture humaine reste **obligatoire**
  avant de soumettre : l'IA assist, elle ne garantit pas.
