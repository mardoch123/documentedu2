---
id: 14-05-rapports-excel-pdf
partie: 14
titre_partie: "Cartes, certificats & rapports"
app: web
slug: 14-05-rapports-excel-pdf
emoji: "📊"
titre: "Rapports : élèves, profs, staff, examens, dépenses, revenus"
resume: "Le module Reports (Rapports) est le centre d'analyse de l'école : il regroupe des tableaux croisés filtrables (par classe, matière, période…"
audiences: [school_admin, staff]
---
# 📊 Rapports : élèves, profs, staff, examens, dépenses, revenus

## 🎯 Rôle
Le module **Reports (Rapports)** est le **centre d'analyse** de l'école : il regroupe des
**tableaux croisés** filtrables (par classe, matière, période…) sur **les élèves**
(résultats, présences, devoirs, journal, transport), **les enseignants** (présences, congés),
**le personnel**, **les examens**, **les dépenses** et **les revenus**. Chaque rapport se
**consulte à l'écran**, se **fouille** (recherche bootstrap-table) et s'**exporte**.

## ✅ Prérequis
1. Avoir saisi les **données de base** (élèves notés, présences pointées, dépenses/revenus
   enregistrés) : un rapport vide vient d'un **travail non fait**, pas d'un bug.
2. Permissions de consultation. Accès : menu **Reports** (sous-menu par catégorie).

## 🟢 Consulter un rapport (étape par étape)
1. Ouvrez **Reports** puis la catégorie voulue :
   - **Élèves** : `reports.student.student-reports` (général),
     **Attendance** (`reports.student.attendance.report`), **Exam**
     (`reports.student.exam.report`), **Assignment** (`reports.student.assignment.report`),
     **Diary** (`reports.student.diary.report`), **Transport attendance**
     (`reports.student.transportation_attendance.report`) ;
   - **Enseignants** : `reports.teacher.teacher-reports`, **Attendance**, **Leave** ;
   - **Personnel** : `reports.staff.staff-reports` ;
   - **Examens** : `reports.exam.exam-reports`, **Yearly result**
     (`reports.exam.yearly-result-show`) ;
   - **Dépenses** : `reports.expense.list` ; **Revenus** : `reports.income.list`.
2. **Filtrez** (classe/section, période, type) puis **Validez** : le tableau se recalcule.
3. Cliquez une **ligne** pour le **détail** (ex. `…student-reports/show`, un élève précis).

## 📤 Exporter / imprimer
- Boutons **bootstrap-table** au-dessus du tableau : **Export Excel / CSV / PDF / Imprimer**.
- Les colonnes visibles s'exportent : **choisissez les colonnes** (icône colonnes) avant.

## 🔎 Recherche
- **Barre de recherche** du tableau : filtre instantanément les lignes déjà chargées.

## ✏️ Modifier / 🔴 Supprimer / ♻️ Restaurer
- **Rien à créer/supprimer ici** : un rapport est une **vue calculée** des données. Pour
  « corriger » un rapport, **corrigez la donnée source** (note, présence, dépense…) dans son
  module ; le rapport se **recalcule** à la réouverture.

## ⚠️ Bon à savoir
- **La donnée source commande le rapport** : note absente = colonne vide ; réglage de
  barème modifié = % recalculés.
- **Yearly result** agrège **les deux/trimestres** : vérifiez que chaque **semestre** est
  clôturé avant de le produire pour l'année.
- **Dépenses/Revenus** : les totaux dépendent des **catégories** choisies en filtre.
- **Exports officiels PDF** : pour les **listes nominatives** (administratif), voir
  *06-telechargement-pdf-listings.md*.
- **Ministère/EducMaster** : des rapports **spéciaux** existent dans le module Académique
  (Rapports Ministériels).
