---
id: 06-10-parents-tuteurs
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-10-parents-tuteurs
emoji: "👨‍👩‍👧"
titre: "Gérer les parents / tuteurs (Guardians)"
resume: "Un parent / tuteur (Guardian) est l'adulte responsable d'un ou plusieurs élèves : père, mère, tuteur."
audiences: [school_admin, staff]
---
# 👨‍👩‍👧 Gérer les parents / tuteurs (Guardians)

## 🎯 Rôle
Un **parent / tuteur (Guardian)** est l'adulte responsable d'un ou plusieurs élèves : père,
mère, tuteur. C'est **par son compte** que la famille reçoit les notifications (notes,
absences, frais, WhatsApp/SMS) et se connecte à l'application parent. Ce module centralise
la liste des parents de l'école et permet de les **créer, rattacher aux élèves, corriger,
activer/couper leurs SMS**.

## ✅ Prérequis
1. Avoir des **élèves** déjà admis.
2. Permission « guardian-create ».
3. Accès : menu **Élèves → Parents / Tuteurs (Guardian)** (icône 👥).

## 📋 Consulter / chercher un parent
1. Ouvrez **Élèves → Gérer les Parents (Guardian)**.
2. Filtrez par **Classe ★** puis **Classe-Section ★** : la liste des parents de ce groupe
   s'affiche (un parent peut avoir plusieurs enfants).
3. Utilisez la **recherche** pour taper un nom ; les colonnes affichent nom, email, mobile,
   sexe, photo et le nombre/lien vers les enfants.

## 🟢 Créer un nouveau parent
1. Bouton **« Créer / Ajouter »** (ou passez par l'étape 4 de l'admission d'un élève qui
   propose « Créer un nouveau parent »).
2. Remplissez le formulaire :
   - **Prénom ★**, **Nom ★**,
   - **Email ★** (c'est l'identifiant de connexion du parent ; laissez le champ « Générer
     automatiquement » cocher s'il n'a pas d'email réel),
   - **Mobile ★** (numéro WhatsApp/SMS — très important pour les notifications),
   - **Sexe ★** (Masc/Fem → Père / Mère / Tuteur),
   - **Photo** (facultatif).
3. **Soumettre**. Le parent est créé ; rattachez-le à l'élève(s) si demandé.

## 🔗 rattacher un parent à un élève
- Depuis la **fiche de l'élève** (Info Apprenant → Modifier → étape Parent), choisissez
  **« Rechercher un parent existant »** et tapez son nom pour l'associer.
- Plusieurs élèves peuvent partager **le même parent** (fratrie) : une seule fiche parent.

## ✏️ Modifier un parent
1. Listes des parents (après filtre classe) → **crayon ✏️** sur la ligne.
2. Le formulaire s'ouvre **pré-rempli** (champ caché `edit_id`) ; corrigez nom, email, mobile,
   sexe ou photo.
3. **Mettre à jour**. La correction s'applique à tous ses enfants rattachés.

## 📴 Couper / réactiver les SMS d'un parent
Deux actions disponibles sur un parent :
- **« disable-sms »** : arrête l'envoi de SMS à ce parent (ex. numéro erroné, plainte).
- **« enable-sms »** : réactive les SMS.
Pensez à **réactiver** après avoir corrigé un numéro, sinon la famille ne reçoit plus rien.

## 🔴 Supprimer un parent
1. Sur la ligne du parent, icône **poubelle 🗑** → confirmez.
⚠️ Vérifiez qu'**aucun élève actif** n'est encore rattaché à ce parent avant de supprimer :
sinon l'élève se retrouve sans contact responsable (notifications orphelines).

## ♻️ Restaurer un parent supprimé
⚠️ Le module Parents **n'a pas de corbeille de restauration** : un parent supprimé ne revient
pas automatiquement. En cas d'erreur, il faut **recréer** le parent (mêmes nom/email/mobile)
puis le **rattacher** à ses enfants. Préférez donc la **modification** (corriger le mobile par
exemple) à la suppression.

## ⚠️ Bon à savoir
- **Un parent propre = des notifications qui arrivent** : le **mobile** est le champ vital
  (WhatsApp/SMS) ; contrôlez le format du numéro.
- **Un seul parent (ou deux)** par élève suffit ; les deux peuvent suivre le même enfant.
- L'**email généré** (badge « Généré ») est un simple identifiant de connexion ; si le parent
  a un vrai email, saisissez-le pour qu'il reçoive aussi les avis par mail.
- Les parents sont **partagés par fratrie** : avant d'en créer un nouveau, **cherchez-le**
  (bouton de recherche) pour éviter les doublons de la même famille.
