---
id: 09-08-moyennes-de-passage
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-08-moyennes-de-passage
emoji: "⚖️"
titre: "Moyennes de passage (calcul de délibération / seuil de réussite)"
resume: "Les « Moyennes de passage » servent à calculer, pour une classe et un trimestre, la moyenne générale de chaque élève et à déterminer qui passe / est admis et qui est ajourné / redouble, selon la mo..."
audiences: [school_admin]
---
# ⚖️ Moyennes de passage (calcul de délibération / seuil de réussite)

## 🎯 Rôle
Les **« Moyennes de passage »** servent à **calculer, pour une classe et un trimestre, la
moyenne générale de chaque élève** et à déterminer qui **passe / est admis** et qui est
**ajourné / redouble**, selon la moyenne minimale de réussite. C'est l'outil du
**conseil de classe / de la délibération** : on obtient un **classement** (rang), une **mention**, un
**statut**, et on peut **exporter le tout en PDF** pour la réunion.

## ✅ Prérequis
1. Avoir **saisi et publié les notes** des examens du trimestre (*02*, *06*).
2. Avoir défini les **mentions/grades** (*09*) pour la conversion moyenne → mention.
3. Permission « view-exam-marks » / « exam-result ».
4. Accès : menu **Offline Exam → Moyennes de passage** (`passing-averages.index`).

## 🟢 Calculer les moyennes de passage (étape par étape)
1. Ouvrez **Moyennes de passage** (sous-titre : *« Définissez les moyennes minimales de
   réussite par classe. »*).
2. Sélectionnez :
   - **« Classe »** ★ ;
   - **« Semestre »** ★ (le trimestre à délibérer).
3. Cliquez **« Calculer les moyennes »**.
4. Le tableau **« Moyennes de Passage »** s'affiche avec, par élève :
   - **Nom de l'apprenant** ;
   - **Moyenne Générale** ;
   - **Rang** ;
   - **Statut** (admis / non admis selon le seuil de la classe) ;
   - **Mention** ;
   - **Détails par matière** (relevé matière par matière).
5. Ajustez éventuellement le **seuil / moyenne minimale** de la classe si l'interface le
   propose : le **statut** se recalcule en conséquence.

## 📤 Exporter pour la délibération
1. Après calcul, le bouton **« Exporter en PDF »** apparaît.
2. Cliquez-le : la **liste des moyennes / statuts / rangs** de la classe se télécharge en
   **PDF**, prête pour le **conseil de classe**.

## ✏️ Recalculer après correction
- Si une note change (re-saisie puis **re-publication** de l'examen, *06*), **relancez
  « Calculer les moyennes »** : les moyennes, rangs et statuts sont **recalculés**.

## 🔴 / ♻️ Supprimer ou restaurer
- Ce calcul est **généré à la demande** : il n'y a **pas d'enregistrement à supprimer** ni de
  corbeille. On **recalcule** quand les données sous-jacentes changent.
- Pour corriger une moyenne fausse : corrigez la **note source** (dépublier → re-saisir →
  re-publier, *06*), puis **recalculez**.

## ⚠️ Bon à savoir
- **Ne pas confondre** avec la **Promotion en masse** (menu Élèves) : la promotion, elle,
  **change réellement la classe** des élèves admis ; les **Moyennes de passage** sont un
  **outil de calcul et de décision** (délibération), sans déplacer les élèves.
- Le **statut** dépend de la **moyenne minimale de réussite** de la classe : renseignez-la
  pour une délibération juste.
- Le **rang** est calculé **au sein de la classe** sélectionnée.
- Les **notes doivent être publiées** pour être comptées : une matière non publiée est
  absente du calcul.
- Exportez le **PDF après chaque recalcul** pour garder la trace de la délibération.
