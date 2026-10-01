---
id: 08-01-pointage-presences-eleves
partie: 8
titre_partie: "Présences & communication"
app: web
slug: 08-01-pointage-presences-eleves
emoji: "✅"
titre: "Pointer les présences des élèves (par classe et par date)"
resume: "Remplacer le feuille d'appel papier : pour une classe et une date données, cocher la position de chaque élève (présent / absent / en retard) et valider."
audiences: [school_admin, teacher, staff]
---
# ✅ Pointer les présences des élèves (par classe et par date)

## 🎯 Rôle
Remplacer le feuille d'appel papier : pour **une classe et une date données**, cocher la
position de chaque élève (présent / absent / en retard) et valider. En cas d'absence, le
logiciel peut **notifier automatiquement le parent par SMS** — la famille sait dans la minute
que son enfant n'est pas arrivé.

## ✅ Prérequis
1. Être **professeur principal de la classe** (« class-teacher ») ou avoir la permission
   « attendance-create ».
2. La **classe/section** et ses élèves doivent exister.
3. L'option d'abonnement **« Attendance Management »** est active (sinon le menu est masqué 🔒).
4. Accès : menu **Présences → Ajouter la présence** (add_attendance).

## 🟢 Faire l'appel (étape par étape)
1. Ouvrez **Présences → Ajouter la présence**.
2. Sélectionnez la **Classe / Section** ★.
3. Choisissez la **Date** ★ (le calendrier n'autorise que le jour même ou une date passée —
   pas le futur).
4. *(Facultatif)* Sélectionnez le **créneau d'emploi du temps** (« timetable ») si vous faites
   l'appel **par cours** plutôt que par journée.
5. La **liste des élèves** se charge (N° d'admission, Matricule, Nom).
6. Pour chaque élève, cochez la position dans la colonne **Type** :
   **present** (présent) · **absent** (absent) · retard s'il est proposé.
7. ⚡ Gain de temps : si toute la classe est là, cochez tout le monde en « présent » sauf les
   absents (toujours plus rapide de pointer les exceptions).
8. Cochez la case **« Envoyer une notification au parent si l'élève est absent »** si vous
   voulez que les SMS partent automatiquement.
9. Cliquez sur **Soumettre** (le bouton apparaît dès que la liste est chargée).
10. Jour de **congés/férié** ? Cochez la case **« holiday »** : la journée est enregistrée
    comme jour férié pour la classe, sans pointer chaque élève.

## ✏️ Corriger un appel (mauvais pointage)
1. **Présences → Ajouter la présence** : même classe, **même date** que l'appel à corriger.
2. La liste se recharge **avec le pointage déjà en place** : remettez les bonnes positions.
3. **Soumettre** à nouveau : l'ancien pointage de ce jour-là est **remplacé**.
> Refaire l'appel d'une date corrigé = pareil que le premier pointage, il n'y a pas de
> « validation » supplémentaire.

## 🔴 Supprimer un pointage / Annuler
- Il n'y a pas de poubelle par ligne de présence : pour « annuler » un appel (ex. appel fait
  par erreur un jour de fermeture), **repointez la même classe/date en cochant « holiday »**
  ou remettez tout le monde « présent » selon le cas réel.
- La correction **rétroactive** reste possible tant que la date est passée : assumez-la
  rapidement pour que les statistiques mensuelles restent justes.

## ♻️ Restaurer des présences perdues
Le pointage ne se « restaure » pas seul : si des élèves ont disparu de la liste, vérifiez
qu'ils sont toujours **actifs** dans la classe (onglet Inactive de **Info Apprenant**) puis
repointez la journée.

## ⚠️ Bon à savoir
- **Faites l'appel à heure fixe** (début de matinée ou 1er cours) : les SMS parents partent
  au moment où la famille peut encore réagir.
- Un élève **souvent absent** : croisez avec le module **Prédictions IA / décrochage**
  (*04-academique-outils-ia/04-decrochage-scolaire-ia.md*).
- Les totaux comptent dans **Présences → Vue** et **Mensuel** (voir *02-consulter-presences.md*)
  et sur les bulletins si votre modèle l'affiche.
- Notification parent : nécessite des **numéros de parent valides** (module Guardians) et un
  crédit SMS actif.
