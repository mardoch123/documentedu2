---
id: 06-01-liste-et-fiche-eleve
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-01-liste-et-fiche-eleve
emoji: "👥"
titre: "Liste des élèves et fiche complète (Info Apprenant)"
resume: "C'est l'écran que vous utiliserez tous les jours : la liste vivante de tous vos élèves, avec en un coup d'œil qui est présent, qui a payé, qui est en transfert."
audiences: [school_admin, staff]
---
# 👥 Liste des élèves et fiche complète (Info Apprenant)

## 🎯 Rôle
C'est **l'écran que vous utiliserez tous les jours** : la liste vivante de tous vos élèves,
avec en un coup d'œil qui est présent, qui a payé, qui est en transfert. En cliquant sur un
élève, vous ouvrez sa **fiche complète** : identité, classe, parents, paiements, documents.

## ✅ Prérequis
1. Avoir au moins une **classe/section** créée (voir *03-academique-structure/07-classes.md*).
2. Avoir déjà admis des élèves (voir *02-admettre-un-eleve.md*).
3. Permission « student-list ».
4. Accès : menu **Élèves → Info Apprenant**.

## 🟢 Comment trouver un élève (étape par étape)
1. Ouvrez **Élèves → Info Apprenant**.
2. La liste affiche tous les élèves avec : **Nom + Email**, badges de statut de frais
   (**Frais payés** vert / **Frais partiels** jaune / **Frais non payés** rouge), et éventuellement
   **Transfert en cours** (jaune) ou **Apprenant transféré avec succès** (vert, nom barré).
3. Pour chercher rapidement : tapez 2-3 lettres dans la **case de recherche** au-dessus du
   tableau (elle cherche dans toutes les colonnes) → la liste se filtre instantanément.
4. Pour trier : cliquez sur l'**en-tête d'une colonne** (petite flèche ↑↓).
5. Pour changer le nombre de lignes affichées : le sélecteur en bas (5, 10, 20, 50, 100, 200).

## 📄 Comment lire la fiche d'un élève
1. **Cliquez sur le nom de l'élève** (en bleu) dans la liste.
2. Un panneau d'actions s'ouvre, donnant accès à la **fiche complète** et aux actions :
   Modifier, Transférer, Désactiver/Activer, PDF du dossier, Carte d'identité, etc.
3. La fiche regroupe : identité (photo, nom, dates), scolarité (classe, section, matricule),
   le/la **parent/tuteur** avec téléphones, l'état des **frais**, et l'historique.

## 🔍 Les outils du tableau (barre en haut à droite)
- 🔎 **Recherche** : filtre instantané.
- 📤 **Export** : télécharger la liste affichée en Excel ou PDF (précisez d'abord vos filtres).
- 🧭 **Colonnes** : afficher/masquer des colonnes (ex. masquer « Email » pour une liste simple).
- ↻ **Rafraîchir** : recharger les données (après une modification par un collègue).

## ✏️ Modifier un élève
1. Listes des élèves → **crayon ✏️** sur la ligne (ou via le panneau d'actions après clic sur le nom).
2. Le formulaire d'admission se rouvre, **pré-rempli** : corrigez seulement les champs utiles.
3. Cliquez sur **Soumettre / Mettre à jour**. Vérifiez que la liste affiche la correction.
→ Toutes les règles du formulaire sont détaillées dans *02-admettre-un-eleve.md*.

## 🔴 Désactiver ou supprimer un élève
Pour les élèves, il existe **DEUX niveaux** différents — comprenez bien la différence :

**A) DÉSACTIVER (recommandé, réversible en 1 clic)** — l'élève part dans l'onglet « Inactive »
mais garde tout son historique (notes, présences, paiements) :
1. Cochez la **case** de l'élève (ou plusieurs) dans la liste.
2. Le bouton **« Inactive »** au-dessus de la liste s'allume → cliquez dessus.
3. L'élève disparaît de l'onglet **active**. Il est « mis en veille », pas effacé.

**B) SUPPRIMER (à ne pas faire sans raison grave)** — via la poubelle 🗑 de la ligne ou le
bouton « Supprimer la sélection » : l'élève est retiré du logiciel.
⚠️ Contrairement aux classes, un **élève supprimé n'a pas de corbeille de restauration
visible** dans ce module : on ne peut pas le « ressortir » soi-même. Privilégiez toujours
la **désactivation** (A). En cas de suppression accidentelle, contactez le **Support EduEasy**.

## ♻️ « Restaurer » un élève = le réactiver
C'est la bonne nouvelle de la désactivation : elle s'annule quand on veut.
1. En haut de la liste, cliquez sur l'onglet **« Inactive »** (à côté de « active »).
2. Cochez la case de l'élève à faire revenir.
3. Le bouton devient **« Active »** → cliquez dessus → confirmez.
4. Retournez dans l'onglet **« active »** : l'élève est revenu, **toutes ses données intactes**.

> Astuce : cette bascule **active ↔ Inactive** est la façon normale de « retirer / remettre »
> un élève (redoublement, départ temporaire, doublon créé par erreur, etc.).

## ⚠️ Bon à savoir
- **Jamais de doublon sans le savoir** : avant d'admettre, cherchez toujours le nom dans
  cette liste (la fiche d'admission signale aussi les homonymes).
- Un élève **transféré avec succès** reste visible (nom barré) pour l'historique de l'année :
  ne le supprimez pas, sinon plus de trace pour les attestations.
- Un élève en **double** créé par erreur : **désactivez-le** (onglet Inactive) plutôt que de
  le supprimer — aucun risque et annulable.
- Le nombre d'élèves **actifs** compte pour votre **abonnement** ; les inactifs aussi selon
  votre forfait : désactivez les départs pour garder des compteurs justes.
- Besoin d'une liste par classe ? Filtrez d'abord par classe, **puis Export** — l'export
  suit les filtres actifs.
