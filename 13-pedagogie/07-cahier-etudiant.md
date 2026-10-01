---
id: 13-07-cahier-etudiant
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-07-cahier-etudiant
emoji: "📖"
titre: "Cahier journal de l'élève (Student Diary)"
resume: "Le cahier journal (student diary) est le carnet de correspondance numérique de chaque élève : on y consigne des observations, des messages aux parents, des notes de vie scolaire datées et classées ..."
audiences: [school_admin, teacher]
---
# 📖 Cahier journal de l'élève (Student Diary)

## 🎯 Rôle
Le **cahier journal** (student diary) est le **carnet de correspondance numérique** de chaque
élève : on y consigne des **observations**, des **messages aux parents**, des **notes de vie
scolaire** datées et classées par **catégorie**. Les **parents** (et l'app mobile) peuvent
retrouver ces entries. Ce module contient deux parties : les **catégories** (les types
d'entrées) et les **entrées elles-mêmes**. Cycle complet avec **corbeille + restauration pour
les catégories**.

## ✅ Prérequis
1. Avoir **classes, sections, matières** et **élèves** inscrits.
2. Abonnement avec la fonction **« Student Diary Management »** activée.
3. Permissions « student-diary-* ». Accès : menu **Student Diary** →
   **Diary Category** (`diary-categories.index`) et **Manage Diaries** (`diary.index`).

## 🗂️ Créer une catégorie (étape par étape)
1. Ouvrez **Student Diary → Diary Category**.
2. Cliquez sur **« Ajouter »** (`diary-categories.create`).
3. Saisissez le **nom de la catégorie** (ex. : *Comportement*, *Devoir non fait*,
   *Félicitation*, *Message parent*).
4. **Enregistrez** (`diary-categories.store`). La catégorie devient un **motif** disponible.

## 🟢 consigner une entrée dans le cahier (étape par étape)
1. Ouvrez **Student Diary → Manage Diaries** → **« Ajouter »** (`diary.create`).
2. Choisissez :
   - la **classe / section** (les matières s'ajustent automatiquement,
     `diary.changeSubjectsByClassSection`) ;
   - l'**élève** concerné (`diary.showStudents`) ;
   - la **catégorie** créée plus haut ;
   - la **date** et le **message / observation**.
3. **Enregistrez** (`diary.store`). L'entrée est **horodatée** et visible selon les droits.

## ✏️ Modifier
- **Catégorie** : icône **Modifier** (`diary-categories.edit`) → `diary-categories.update`.
- **Entrée** : icône **Modifier** (`diary.edit`) → `diary.update` (corrigez le message).

## 🔴 Supprimer
- **Catégorie** : icône **Supprimer** (`diary-categories.trash`) → part à la **corbeille**.
- **Entrée** : icône **Supprimer** (`diary.destroy`) → **disparaît définitivement**.
- **Retirer un élève** d'une entrée (`diary/{diaryId}/remove-student/{id}`) sans supprimer
  l'entrée elle-même.

## ♻️ Restaurer
- **Catégories : restaurables.** Basculez le filtre **« all | Trashed »** sur **« Trashed »**,
  puis **Restaurer** (`diary-categories.restore`) → la catégorie **revient**.
- ⚠️ **Entrées de cahier : non restaurables.** Une entrée supprimée est **perdue** : il faut la
  **reconsigner**. Notez l'important avant de supprimer.

## ⚠️ Bon à savoir
- **Catégories = modèles** : créez-les **d'abord**, elles alimentent le menu déroulant des
  entrées.
- **Traçabilité** : chaque entrée porte une **date** — utile en cas de litige avec un parent.
- **Ne supprimez pas une entrée ancienne** sans certitude : pas de corbeille pour les entrées.
- Les **parents** consultent ces messages via leur **espace / app mobile**.
- Pour le **cahier de vacances** (travail à faire pendant les congés), c'est un autre module :
  voir *08-jours-feries.md* (Cahiers de Vacances IA).
