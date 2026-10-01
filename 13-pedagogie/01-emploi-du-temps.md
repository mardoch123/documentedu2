---
id: 13-01-emploi-du-temps
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-01-emploi-du-temps
emoji: "🗓️"
titre: "Emploi du temps : créer et consulter"
resume: "L'emploi du temps découpe la semaine de chaque classe en créneaux (jour + heure) occupés par une matière enseignée par un professeur, dans une salle."
audiences: [school_admin, teacher]
---
# 🗓️ Emploi du temps : créer et consulter

## 🎯 Rôle
L'**emploi du temps** découpe la semaine de chaque **classe** en **créneaux** (jour + heure)
occupés par une **matière** enseignée par un **professeur**, dans une **salle**. Il sert de
**référence** aux cours, aux présences du jour et à la **feuille de route des enseignants**.
Le module accepte même une **import par photo/OCR** (scanner un emploi du temps papier).

## ✅ Prérequis
1. Avoir **classes/sections, matières, professeurs, salles** déjà créés.
2. Une **période / semestre** actif.
3. Permission « timetable ». Accès : menu **Timetable** (`timetable.index`).

## 🟢 Créer un emploi du temps (étape par étape)
1. Ouvrez **Timetable** → **« Ajouter »** (`timetable.create`).
2. Choisissez la **classe/section** (et le **semestre**) concernés.
3. **Remplissez la grille** de la semaine : pour chaque **jour** et **créneau horaire**,
   affectez une **matière** + un **professeur** (+ salle éventuelle).
4. Respectez les **règles** (pas de doublon prof/créneau, pas de chevauchement de classe).
5. **Enregistrez** (`timetable.store`). L'emploi du temps devient la **trame officielle** de
   la classe.

## 📸 Import rapide par OCR (photo/scan)
1. Dans l'éditeur, utilisez **« Extraire par IA/OCR »** (`timetable.ai-ocr-extract`) : envoyez
   une **image/PDF** d'un emploi du temps existant.
2. Le logiciel **reconnaît les créneaux** ; vérifiez-les puis **« Appliquer »**
   (`timetable.apply-ocr-slots`) pour les **injecter** dans la grille.

## 👀 Consulter
- **Par classe** : la grille hebdomadaire s'affiche (imprimable).
- **Par enseignant** : chaque prof voit **SON** emploi du temps (`timetable.teacher.index`,
  `timetable.teacher.show`) — ses heures de cours de la semaine.
- L'emploi du temps **alimente la présence du jour** (les créneaux du jour proposent
  l'appel).

## ✏️ Modifier
1. Icône **Modifier** (`timetable.edit`) → déplacez/ajoutez/supprimez des **créneaux**.
2. **Enregistrez** (`timetable.update`).

## 🔴 Supprimer
1. Icône **Supprimer** (`timetable.destroy`), confirmez → l'emploi du temps est **retiré**.

## ♻️ Restaurer
- ⚠️ Les **emplois du temps ne sont pas restaurables** (pas de corbeille) : une suppression
  impose de **re-créer** la grille (ou de la **ré-importer par OCR** si vous avez la photo).
  **Sauvegardez** une copie (PDF/photo) avant toute suppression.

## ⚠️ Bon à savoir
- **Un créneau = matière + prof + heure + jour** ; la même matière apparaît plusieurs fois
  par semaine selon le volume horaire.
- **Conflits** : le logiciel refuse un prof doublement occupé sur un même créneau.
- L'**OCR** fait gagner un temps énorme en **rentrée** : scannez l'ancien emploi du temps.
- Le **professeur** consulte le sien pour savoir **quand il a cours** ; l'appel se fait sur
  ce créneau.
- Lié aux **leçons** (*03*) : le prof déclare ses **contenus de cours** par créneau/matière.
