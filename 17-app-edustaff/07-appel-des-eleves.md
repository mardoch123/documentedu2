---
id: 17-07-appel-des-eleves
partie: 17
titre_partie: "Application EduStaff"
app: edustaff
slug: 17-07-appel-des-eleves
emoji: "📋"
titre: "faire l'appel et consulter les présences des élèves"
resume: "Enregistrer la présence des élèves séance par séance (présent / absent / en retard), prévenir automatiquement les parents par notification, et relire l'historique des appels déjà"
audiences: [teacher, staff, school_admin]
---
# 📋 17.7 — EduStaff : faire l'appel et consulter les présences des élèves

## 🎯 Rôle
Enregistrer la **présence des élèves** séance par séance (présent / absent / en
retard), prévenir automatiquement les **parents par notification**, et relire
l'historique des appels déjà saisis.

## ✅ Prérequis
1. Être connecté à EduStaff (page 17.1) et avoir des classes affectées (page 17.6).
2. Que le module **présence des élèves** soit actif pour l'école (PARTIE 08).
3. Pour l'envoi aux parents : que les numéros des tuteurs soient renseignés dans les
   fiches élèves.

## 🟢 Faire l'appel (étape par étape)
1. Accueil → tuile **« Faire l'appel »** (« Add Attendance »).
2. Choisissez la **classe/section** dans le premier filtre.
3. Choisissez la **date** (par défaut : aujourd'hui) — utile pour rattraper un appel
   oublié la veille.
4. Choisissez le **cours** (la matière/séance du moment) dans le menu « Cours ».
5. La liste des **élèves actifs** de la classe s'affiche, tous marqués « présent »
   par défaut.
6. Touchez le statut des exceptions : **absent**, **en retard**, selon les cases
   proposées.
7. Si c'est un jour sans classe officiel, activez l'option **« jour férié »** :
   l'appel est enregistré comme tel.
8. Laissez cochée **« Envoyer une notification aux parents des élèves absents »** pour
   que chaque tuteur prévenu reçoive l'alerte automatiquement.
9. Appuyez sur **Enregistrer** : message de confirmation, l'appel est compté.

## 🟢 Relire les appels (Voir la présence)
1. Tuile **« Voir la présence »** (« View Attendance »).
2. Filtres : **classe**, **date**, et **statut** (tous / présents seulement / absents).
3. La liste du jour choisi s'affiche avec le statut de chaque élève ; balayez les
   jours avec le sélecteur de date.
4. Message « Aucune présence » : aucun appel n'a été saisi pour ce couple
   classe/date — refaites l'appel (section ci-dessus).

## ✏️ Modifier un appel
1. Refaites le circuit **« Faire l'appel »** avec la **même classe, la même date et
   le même cours**.
2. Ajustez les statuts ; **enregistrez** à nouveau : l'appel existant est **remplacé**
   par la nouvelle saisie (pas de doublon).
3. Prévenez les parents vous-même si l'erreur avait déclenché une notification
   injustifiée.

## 🔴 Supprimer / effacer
- Pas de bouton « supprimer l'appel » dans l'app : on **remplace** la saisie comme
  décrit ci-dessus, ou la direction annule la ligne sur le web (PARTIE 08).

## ♻️ Restaurer
- Élève absent de la liste d'appel : il est peut-être **inactif, transféré ou
  suspendu** — vérifiez sa fiche (page 17.6) ; remettez-le actif sur le web pour
  qu'il revienne dans l'appel.
- Appel perdu (téléphone éteint avant Enregistrer) : recommencez, rien n'était sauvé
  à mi-chemin.
- Notifications parents non parties : numéros manquants ou module SMS/WhatsApp de
  l'école hors quota — signalez à la direction (PARTIE 08).

## ⚠️ Bon à savoir
- Faites l'appel **en début de séance** : la notification aux parents part à la
  validation, un retard d'appel = un retard d'alerte.
- L'option « notification aux parents » s'applique **par enregistrement** : décochez-la
  si vous corrigez un appel pour éviter de re-prévenir les parents.
- Les statistiques de présence (taux, courbes) se consultent sur le web ; l'app ne
  donne que la saisie et la lecture par jour.
- Un élève porté absent **à tort** puis corrigé : l'historique web garde la trace de la
  modification — pas d'inquiétude pour le bulletin de fin de trimestre, la dernière
  valeur compte.
