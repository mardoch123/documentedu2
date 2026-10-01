---
id: 13-06-fiches-de-cours
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-06-fiches-de-cours
emoji: "📋"
titre: "Fiches de préparation de cours (profs) + validation direction"
resume: "La fiche de préparation (course sheet) est le document pédagogique qu'un enseignant prépare avant son cours (objectifs, contenu, déroulé, méthodes, évaluation)."
audiences: [school_admin, teacher]
---
# 📋 Fiches de préparation de cours (profs) + validation direction

## 🎯 Rôle
La **fiche de préparation** (course sheet) est le **document pédagogique** qu'un enseignant
**prépare avant son cours** (objectifs, contenu, déroulé, méthodes, évaluation). Elle est
**soumise à la direction**, qui la **valide ou la renvoie**. C'est l'outil de **suivi
qualité** de l'enseignement. ⚠️ Module **payant à crédits** (comme le générateur IA), avec
export **PDF**.

## ✅ Prérequis
1. Être **enseignant** (création) / **direction** (validation).
2. Avoir **classe + matière** et des **leçons** (*03*).
3. Disposer de **crédits** si le module est facturé (`course-sheets.usage-stats`).
4. Accès : menu **Course Sheets** (`course-sheets.index`).

## 🟢 Préparer une fiche de cours (étape par étape)
1. Ouvrez **Course Sheets** → **« Nouvelle fiche »** (`course-sheets.create`).
2. Choisissez la **classe/section**, puis la **matière**
   (`course-sheets.subjects-by-class/{class_section_id}`).
3. **Générez** la trame (`course-sheets.generate`) ou remplissez la fiche : **objet de la
   leçon, objectifs, déroulement, supports, évaluation**.
4. **Enregistrez** (`course-sheets.store`). La fiche est en brouillon.

## 📤 Soumettre à la direction (workflow)
1. Une fois la fiche prête, l'enseignant la **soumet** (`course-sheets.submit/{id}`).
2. Statut → **« en attente de validation »**.

## ✅ Valider / renvoyer (direction)
1. La direction ouvre la fiche soumise (`course-sheets.show/{id}`).
2. Elle **approuve** (`course-sheets.approve/{id}`) — la fiche est **validée** — ou
   **rejette** (`course-sheets.reject/{id}`) avec des remarques → l'enseignant **corrige**
   (`course-sheets.edit/{id}` → `update`) puis **re-soumet**.

## 🖨️ Imprimer / exporter
- **Générer le PDF** de la fiche (`course-sheets.pdf/{id}`) pour archivage ou remise.

## 💳 Paiement / crédits
- **Statistiques d'usage** (`course-sheets.usage-stats`) ; si le module est payant :
  **paiement** (`course-sheets.payment`, `payment.initiate`, `payment.process`) pour
  recharger les crédits.

## ✏️ Modifier / 🔴 Supprimer
- **Modifier** une fiche (`course-sheets.edit/{id}` → `course-sheets.update`).
- **Supprimer** (`course-sheets.destroy/{id}`) → la fiche est **retirée**.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** : une fiche supprimée doit être **recréée** (et re-validée).
  **Exportez en PDF** les fiches importantes avant suppression.

## ⚠️ Bon à savoir
- **Cycle clair** : Brouillon → **Soumise** → **Approuvée** / **Rejetée** (retour
  enseignant). Ne sautez pas la **soumission** si la direction doit valider.
- La fiche **s'appuie sur les leçons** (*03*) : gardez le contenu de cours à jour.
- **Rejet ≠ punition** : le rejet invite à **corriger** ; re-soumettez après retouches.
- **Paiement par usage** : surveillez les **crédits** comme pour le générateur IA (*05*).
- **Différent de la leçon** : la *leçon* = ce qui a été **enseigné** ; la *fiche* = le
  **document de préparation** contrôlé par la hiérarchie.
