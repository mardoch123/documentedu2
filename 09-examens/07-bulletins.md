---
id: 09-07-bulletins
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-07-bulletins
emoji: "🧾"
titre: "Générer et imprimer les bulletins de notes"
resume: "Le bulletin rassemble, pour un élève et un trimestre/semestre, ses notes par matière, les coefficients, la moyenne générale, le rang, la mention et les appréciations."
audiences: [school_admin]
---
# 🧾 Générer et imprimer les bulletins de notes

## 🎯 Rôle
Le **bulletin** rassemble, pour un **élève** et un **trimestre/semestre**, ses **notes par
matière**, les **coefficients**, la **moyenne générale**, le **rang**, la **mention** et les
**appréciations**. Cette page permet de **choisir la classe et le trimestre**, d'**ajuster la
formule de calcul et les coefficients**, de **rédiger les appréciations** (y compris par IA),
puis de **générer et télécharger/imprimer** le bulletin en PDF.

## ✅ Prérequis
1. Avoir **publié les résultats** des examens du trimestre concerné (*06*).
2. Avoir configuré **matières + coefficients** et, si besoin, les **mentions/grades** (*09*).
3. Permission « view-exam-marks » / « exam-result ».
4. Accès : menu **Offline Exam → Bulletins** (`bulletins.index`).

## 🟢 Générer un bulletin (étape par étape)
1. Ouvrez **Bulletins** (sous-titre : *« Consultez, générez et imprimez les bulletins de
   notes. »*). L'écran est en **deux volets** : réglages à gauche, **aperçu** à droite.
2. À gauche, choisissez :
   - **« Sélectionner une classe »** ★ ;
   - **« Sélectionner un semestre »** ★ (le trimestre du bulletin).
3. Réglez le **calcul** si nécessaire (carte « Formules & Coefficients ») :
   - **Formule** de moyenne : *Standard Bénin (MI + D1 + D2)/3*, *Avec Composition*,
     *Pondération 40% CC + 60% Composition*, *Moyenne simple* ;
   - **« Coefficients matières »** : attribuez le **coefficient** de chaque matière
     (bouton « Coefficients matières »).
4. Rédigez les **appréciations** (voir plus bas) puis cliquez
   **« Générer & Télécharger »**.
5. L'**aperçu du bulletin** s'affiche à droite ; le **PDF se télécharge / s'imprime**.

## ✍️ Appréciations (dont génération par IA)
1. Dans la carte **« Appréciations IA »**, cliquez **« Rédiger / Gérer »**.
2. Pour aller vite : **« Générer pour toute la classe (IA) »** rédige automatiquement une
   appréciation pour **chaque élève** de la classe à partir de ses notes.
3. **Relisez et personnalisez** chaque appréciation (l'IA propose, l'humain valide), puis
   **Enregistrez** les appréciations.
4. L'appréciation **générale** de l'élève figure sur le bulletin.

## 🔁 Coefficients par classe / matière
- Le bouton **« Coefficients matières »** ouvre la fenêtre de saisie des **coefficients**
  propres à la **classe** sélectionnée ; ils servent au calcul de la moyenne du bulletin.
- Enregistrez : les coefficients sont **mémorisés pour la classe** et réutilisés.

## ✏️ Modifier / régénérer un bulletin
1. Changez la classe, le trimestre, les coefficients ou les appréciations.
2. Cliquez à nouveau **« Générer & Télécharger »** : le bulletin est **recalculé** avec les
   nouvelles données (l'aperçu et le PDF sont régénérés).

## 🔴 / ♻️ Supprimer ou restaurer un bulletin
- Le bulletin **n'est pas un objet que l'on stocke/supprime** : c'est un **document généré à
  la volée** à partir des notes publiées. Il n'y a donc **ni poubelle ni restauration** de
  bulletin.
- Pour « corriger un bulletin diffusé » : **corrigez les notes/coefficients/appéciations**,
  puis **régénérez** le PDF.
- Si les **notes** elles-mêmes sont fausses, **dépubliez** l'examen (*06*), re-saisissez,
  re-publiez, puis régénérez le bulletin.

## 🛡️ Vérification d'authenticité (bonus)
- Chaque bulletin généré porte un **code** et une **signature** : le lien
  `bulletin/verify/{code}/{signature}` permet à un tiers (autre école, parent) de
  **vérifier l'authenticité** du document.
- Un **espace parent** permet d'ajouter une **« observation du parent »** sur le bulletin
  vérifié.

## ⚠️ Bon à savoir
- **Sans résultats publiés**, le bulletin sera **vide ou erroné** : publiez d'abord (*06*).
- Le **choix du trimestre** est indispensable : un bulletin = une classe + un semestre précis.
- La **formule dépend du pays/cycle** (les préréglages « Bénin » couvrent le cas courant) ;
  ajustez les **coefficients** pour coller au règlement de votre établissement.
- La page **Promotion en masse** (*voir Élèves → Promotion*) renvoie vers ce menu **Bulletins**
  pour la suite (relevés, impressions) après le passage de classe.
