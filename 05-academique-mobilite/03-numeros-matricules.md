---
id: 05-03-numeros-matricules
partie: 5
titre_partie: "Académique : Mobilité"
app: web
slug: 05-03-numeros-matricules
emoji: "🔢"
titre: "Numéros de matricules (Roll Numbers)"
resume: "Attribuer ou réorganiser les numéros de matricule (numéro d'ordre de l'élève dans sa classe : 001, 002, 003…"
audiences: [school_admin]
---
# 🔢 Numéros de matricules (Roll Numbers)

## 🎯 Rôle
Attribuer ou réorganiser les **numéros de matricule** (numéro d'ordre de l'élève dans sa
classe : 001, 002, 003…) pour **toute une classe d'un coup**, selon l'ordre de tri de votre
choix (par prénom ou par nom, croissant ou décroissant). C'est beaucoup plus rapide que de
modifier les élèves un par un, et ça garantit une numérotation propre pour les bulletins,
les listes d'appel et les cartes d'identité.

## ✅ Prérequis
1. Avoir créé les **classes/sections** et y avoir déjà **inscrit les élèves**.
2. Permission « student-list » (accès à la liste des élèves).
3. Accès : menu **Académique → Mobilité & Parcours → Numéros de matricules**.

## 🟢 Comment attribuer les matricules (étape par étape)
1. Ouvrez le module **Numéros de matricules**.
2. Dans le filtre **« Class Section »**, choisissez la **classe (et section)** à numéroter.
3. Choisissez l'**ordre de tri** (« sort by ») :
   - **first_name** = ordre alphabétique des prénoms,
   - **last_name** = ordre alphabétique des noms.
4. Choisissez le **sens** (« Order By ») : **Ascending** (A→Z) ou **Descending** (Z→A).
5. La liste des élèves de la classe s'affiche dans cet ordre, avec une **case « Roll Number »
   à remplir sur chaque ligne**.
6. Saisissez les numéros (ex. 001, 002, 003…). ⚠️ **Toutes les cases sont obligatoires** :
   le système refuse l'enregistrement s'il manque un seul matricule.
   Astuce : remplissez la première ligne, puis tapez Entrée/down pour descendre vite.
7. Cliquez sur **Soumettre / Enregistrer**.
8. Vérifiez en rechargeant la liste : les matricules sont appliqués.

## ✏️ Comment modifier les matricules
Reprenez exactement les mêmes étapes : le module affiche les matricules **actuels** dans les
cases ; changez seulement ceux à corriger et **Soumettez** de nouveau. L'opération remplace
la numérotation de la classe, aussi souvent que nécessaire, sans effet secondaire ailleurs
(les notes et présences restent liées à l'élève, pas au numéro).

## 🔴 Supprimer / retirer un matricule
Il n'existe pas de « suppression de matricule » isolée :
- Pour **rendre son numéro à un élève qui part**, supprimez (ou transférez) tout
  simplement sa **fiche élève** (module Élèves → poubelle 🗑), puis relancez ce module pour
  **renuméroter la classe** proprement sans trou.
- Ne laissez jamais une case vide « exprès » pour marquer un départ : le système refusera
  l'enregistrement.

## ♻️ Restaurer après une erreur de numérotation
Une mauvaise saisie se « restaure » en re-numérotant : retournez dans le module, remettez
les bons numbers dans l'ordre voulu, **Soumettez**. Aucune donnée d'élève n'est perdue par
une re-numérotation.

## ⚠️ Bon à savoir
- Travaillez **classe par classe** : le filtre classe est la clé de la page.
- La liste est **exportable** (icône export en haut du tableau) si vous voulez vérifier
  dans Excel avant de valider — mais l'enregistrement se fait bien ici, pas dans Excel.
- Les élèves fraîchement importés en masse n'ont souvent **pas de matricule** : ce module
  est l'étape suivante recommandée après un import ou une rentrée.
- L'ordre choisi ici sert de base aux **listes d'appel imprimées** et à l'ordre sur les
  bulletins dans plusieurs modèles : figez la numérotation tôt dans l'année.
