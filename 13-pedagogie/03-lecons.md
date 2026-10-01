---
id: 13-03-lecons
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-03-lecons
emoji: "📚"
titre: "Leçons (subject lessons) et sujets/topics"
resume: "Une leçon est une séquence de cours déclarée par l'enseignant pour une matière et une classe (titre, contenu, fichiers joints, date)."
audiences: [school_admin, teacher]
---
# 📚 Leçons (subject lessons) et sujets/topics

## 🎯 Rôle
Une **leçon** est une **séquence de cours** déclarée par l'enseignant pour une **matière** et
une **classe** (titre, contenu, fichiers joints, date). Chaque leçon se décline en
**sujets / topics** (les points précis traités). Ce module constitue le **programme réellement
enseigné** — la mémoire de ce qui a été vu en classe. Cycle complet avec **corbeille +
restauration** pour les leçons **et** les topics.

## ✅ Prérequis
1. Avoir **matières, classes/sections, enseignants** et un **semestre** actif.
2. Permission « lesson ». Accès : menu **Lesson** (`lesson.index`).

## 🟢 Créer une leçon (étape par étape)
1. Ouvrez **Lessons** → **« Ajouter »** (`lesson.create`).
2. Renseignez :
   - **Classe/section** et **Matière** ;
   - **Titre de la leçon** ;
   - **Contenu / description** ;
   - **Date** de la séance ;
   - **Fichiers joints** (support de cours, PDF, images…).
3. **Enregistrez** (`lesson.store`). La leçon rejoint le **programme** de la matière.
4. On peut **filtrer par classe** (`lessons.by-class/{class_section_id}`).

## 🧩 Ajouter des sujets / topics
1. Ouvrez une leçon, puis **Topics** (`lesson-topic`).
2. **Ajouter un topic** (`lesson-topic.store`) : un **point du programme** traité dans la
   leçon.
3. **Modifier / supprimer** un topic (`lesson-topic.update` / `lesson-topic.trash`).

## 🔎 Rechercher
- **Recherche de leçons** (`lesson.search`) : retrouver une leçon par titre/matière/classe.

## ✏️ Modifier une leçon
1. Icône **Modifier** (`lesson.edit`) → corrigez titre/contenu/date/fichiers →
   `lesson.update`.
2. **Retirer un fichier** joint (`file.delete/{id}`) sans supprimer la leçon.

## 🔴 Supprimer une leçon (corbeille)
1. Icône **Supprimer** (`lesson.trash`, `lesson/{id}/deleted`), confirmez.
2. La leçon part à la **corbeille** ; basculez **« all | Trashed »** sur **« Trashed »**.
3. Depuis « Trashed », **suppression définitive**.

## ♻️ Restaurer une leçon (ou un topic)
1. Mode **« Trashed »**.
2. **Restaurer** (`lesson.restore`, `lesson/{id}/restore`) → la leçon **revient** avec son
   contenu et ses fichiers.
3. Les **topics** suivent la **même logique** (`lesson-topic.restore`).

## ⚠️ Bon à savoir
- **Leçon ≠ fiche de préparation** : la *leçon* (ici) est **ce qui a été enseigné** ; la *fiche
  de préparation* (*06*) est le **document pédagogique** du prof soumis à la direction.
- **Les leçons nourrissent les devoirs IA** (*05*) : le générateur puise dans vos **leçons**
  pour créer des exercices cohérents (`homework-generator.get-lessons`).
- **Topics = programme détaillé** : utiles pour couvrir un **syllabus** et préparer les
  **examens**.
- **Restauration dispo** : contrairement aux devoirs, une leçon supprimée se **récupère** via
  « Trashed ».
