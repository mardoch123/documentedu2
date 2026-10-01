---
id: 11-01-liste-enseignants
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-01-liste-enseignants
emoji: "👨‍🏫"
titre: "Gérer les enseignants (fiche, photo, matières)"
resume: "Cette page (Manage Teacher) centralise la fiche de chaque enseignant : identité, photo, coordonnées, qualification, mode de rémunération, et affectations (classes et matières qu'il enseigne)."
audiences: [school_admin]
---
# 👨‍🏫 Gérer les enseignants (fiche, photo, matières)

## 🎯 Rôle
Cette page (**Manage Teacher**) centralise la **fiche de chaque enseignant** : identité,
photo, coordonnées, qualification, mode de rémunération, et **affectations** (classes et
matières qu'il enseigne). C'est ici qu'on **inscrit un nouvel enseignant**, qu'on **complète
sa fiche** et qu'on **consulte son détail** (matières + note moyenne donnée par les
élèves/parents via les avis).

## ✅ Prérequis
1. Permission « **teacher-create** » (inscrire) / « teacher-edit » / « teacher-list » /
   « teacher-delete ».
2. Avoir **classes/sections** et **matières** prêtes pour affecter un cours.
3. Accès : menu **Teacher → Manage Teacher** (`teachers.index`).

## 🟢 Inscrire un enseignant (étape par étape)
1. Sur **Manage Teacher**, cliquez **« Ajouter »** (le formulaire d'ajout s'ouvre).
2. Renseignez l'**identité** :
   - **Prénom (first_name)** ★ ;
   - **Nom (last_name)** ★ ;
   - **Sexe (gender)** ★ ;
   - **Email** ★ — **unique** dans le système (sert aussi d'identifiant de connexion) ;
   - **Mobile** ★ (6 à 15 chiffres) ;
   - **Date de naissance (dob)** ★ ;
   - **Qualification** ★ (diplôme / niveau) ;
   - **Adresse actuelle** ★ et **Adresse permanente** ★ ;
   - **Photo (image)** — facultative (jpeg, png, jpg, svg, gif, webp) ;
   - **Statut** — actif / inactif.
3. Renseignez la **rémunération** :
   - **Type de paiement (payment_type)** ★ : **Salaire** (mensuel) ou **Taux horaire** ;
   - **Salaire** ★ si « Salaire », ou **Taux horaire (hourly_rate)** ★ si « Horaire ».
4. **Enregistrez**. L'enseignant apparaît dans la liste et reçoit (selon réglage) une
   **notification** de création de compte.

## 📚 Affecter des classes & matières
1. Ouvrez la **fiche détail** de l'enseignant (`teachers.details/{id}`) : on y voit ses
   **affectations** (classes/sections + matières) et sa **note moyenne** (avis).
2. Les **affectations matière ↔ enseignant** se gèrent depuis les **classes / sections**
   (voir *PARTIE Académique — Classes* et *Affectation des professeurs aux matières*) :
   c'est là qu'on dit « M. X enseigne les Maths en 6ème A ».
3. Pour **professeur principal** d'une classe : voir l'affectation **Class Teacher**
   (acady/`class-teacher`).

## ✏️ Modifier un enseignant
1. Icône **Modifier** sur la ligne (`teachers.edit`).
2. Ajustez identité, photo, rémunération. ⚠️ **L'email doit rester unique** (un email déjà
   pris est refusé).
3. **Enregistrez**.

## 🔴 Supprimer / désactiver / ♻️ Restaurer
> Le cycle complet (suppression corbeille, désactivation par statut, restauration) est
> détaillé dans **03-supprimer-restaurer-enseignant.md**. En bref :
> - **Désactiver** = basculer le **statut** (compte conservé, accès coupé) — recommandé ;
> - **Supprimer** = aller à la **corbeille** (`teachers.trash`) ;
> - **Restaurer** = depuis « Trashed », **Restaurer** (`teachers.restore`).

## ⚠️ Bon à savoir
- **Email = identifiant** : un enseignant se connecte avec cet email ; mettez un email
  **valide et unique**.
- La **fiche détail** affiche les **avis/révisions** approuvés et la **note moyenne** de
  l'enseignant : utile pour l'évaluation du personnel.
- **Salaire vs Horaire** conditionne le calcul de la **paie** (voir *PARTIE 10 — 12-paie* et
  *09-fiches-de-paie-slip*).
- Pour **inscrire beaucoup d'enseignants d'un coup**, utilisez l'**import en masse**
  (*02-ajouter-enseignant-en-masse.md*).
- Un enseignant peut aussi être **fusionné** avec un compte **Staff** (même personne,
  même email) — voir *04*.
