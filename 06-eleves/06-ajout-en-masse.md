---
id: 06-06-ajout-en-masse
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-06-ajout-en-masse
emoji: "📥"
titre: "Ajouter plusieurs élèves d'un coup (import CSV / masse)"
resume: "Inscrire une classe entière en une fois au lieu de refaire 40 formulaires."
audiences: [school_admin, staff]
---
# 📥 Ajouter plusieurs élèves d'un coup (import CSV / masse)

## 🎯 Rôle
Inscrire **une classe entière en une fois** au lieu de refaire 40 formulaires. Vous remplissez
un **fichier tableur** (une ligne = un élève), vous l'envoyez, et le logiciel crée tous les
comptes d'un coup. C'est la méthode idéale à la **rentrée scolaire**.

## ✅ Prérequis
1. Avoir créé la **classe / section** de destination et l'**année de session**.
2. Permission « student-create ».
3. Un fichier **CSV** propre (voir le modèle fourni par le logiciel).
4. Accès : menu **Élèves → Ajouter en masse** (icône 📥).

## 🟢 Méthode conseillée — Import Intelligent IA (le plus simple)
En haut de la page se trouve une **bannière bleue « Nouveau : Import Intelligent Multi-Format
par IA »** (bouton **« Utiliser l'Import Intelligent IA → »**). Si vous partez d'une **liste
papier, d'un PDF, d'une photo ou d'un Word**, cliquez dessus : l'IA lit le document toute
seule. La procédure complète est décrite dans
*04-academique-outils-ia/01-import-intelligent.md*. **C'est la voie recommandée aux
non-techniciens** — pas de formatage de colonnes à faire.

## 🟡 Méthode classique — Fichier CSV (si vous préférez un tableau précis)
1. Sous le formulaire, cliquez sur **« Télécharger le fichier modèle (dummy file) »** :
   un fichier d'exemple avec les bonnes colonnes se télécharge.
2. **Ouvrez-le** et remplissez **une ligne par élève** (Nom, Prénom, Sexe, date de naissance,
   parent, mobile…). Gardez les **en-têtes de colonnes** tels quels.
3. ⚠️ **Enregistrez le fichier au format .CSV** (le logiciel demande explicitement :
   « First download dummy file and convert to .csv file then upload it »).
4. Revenez sur **Élèves → Ajouter en masse**.
5. Choisissez l'**Année de session** ★ (pré-sélectionnée sur l'année courante).
6. Choisissez la **Classe / Section** ★ de destination.
7. Cliquez sur **Parcourir / Upload** ★ et sélectionnez votre fichier .csv.
8. Cases utiles :
   - **« Envoyer une notification »** : prévient les parents par email/SMS de la création.
   - **« Générer automatiquement les emails »** (cochée par défaut) : crée un identifiant de
     connexion pour les parents **qui n'ont pas d'email** dans le fichier. Décochez-la si vos
     emails du CSV sont réels et à conserver.
9. Cliquez sur **Soumettre**.
10. Attendez le rapport : nombre d'élèves créés / ignorés / en erreur.

## ✏️ Corriger après import
Un import crée des **fiches élèves normales**. Toute erreur se corrige donc dans
**Élèves → Info Apprenant** (crayon ✏️), **pas** dans cet écran d'import.
(Re-exportez, corrigez le CSV et ré-importez uniquement si vous voulez tout refaire — voyez
le point suivant sur les doublons.)

## 🔴 Annuler un mauvais import / supprimé la sélection
1. **Élèves → Info Apprenant**, filtrez par la **classe** importée aujourd'hui.
2. Cochez les élèves importés par erreur (ou « tout sélectionner »).
3. Bouton **« Inactive »** pour les mettre en veille **en lot** (réversible) — recommandé.
⚠️ Un import qui a réussi ne se « dé-importe » pas en un clic : on traite les lignes élève
par élève ensuite. **Faites toujours un test avec 3-5 lignes d'abord** pour valider le format.

## ♻️ Retrouver des élèves mal importés puis désactivés
**Info Apprenant → onglet « Inactive »** → cocher → **« Active »** (comme la page
*03-modifier-supprimer-restaurer-eleve.md*).

## ⚠️ Bon à savoir
- **Doublons** : avant un import en masse, vérifiez que ces élèves ne sont pas déjà dans la
  liste (recherche par nom). Un doublon crée deux comptes séparés, très pénibles à fusionner.
- **Accents qui s'abîment** : un CSV mal encodé transforme « Élodie » en « ldie » ; préférez
  le format Excel (.xlsx) via l'**Import IA**, ou enregistrez le CSV en **UTF-8**.
- **Téléphones / matricules** : écrivez-les tels quels dans le fichier ; le logiciel peut les
  lire comme des nombres et effacer un « 0 » de début sinon.
- L'import n'attribue **pas les matricules** : lancez ensuite *05-academique-mobilite/03-numeros-matricules.md*.
