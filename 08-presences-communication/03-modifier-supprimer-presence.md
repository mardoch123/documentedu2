---
id: 08-03-modifier-supprimer-presence
partie: 8
titre_partie: "Présences & communication"
app: web
slug: 08-03-modifier-supprimer-presence
emoji: "✏️"
titre: "Corriger ou annuler une pointe de présence"
resume: "Une erreur d'appel arrive vite (mauvaise case cochée, élève parti malade à midi, oubli de l'appel d'une classe)."
audiences: [school_admin, teacher, staff]
---
# ✏️ Corriger ou annuler une pointe de présence

## 🎯 Rôle
Une erreur d'appel arrive vite (mauvaise case cochée, élève parti malade à midi, oubli de
l'appel d'une classe). Cette page explique **comment reprendre le pointage d'une journée
passée et le corriger**, ou **l'annuler** — en comprenant que le logiciel **écrase** le
pointage précédent plutôt que de le « supprimer ».

## ✅ Prérequis
1. Permission « attendance-create » ou « attendance-edit » (ou être prof principal).
2. Connaître la **classe**, la **date** (et le **créneau** si appel par cours) à corriger.
3. Accès : menu **Présences → Ajouter la présence**.

## 🟢 Corriger un pointage (étape par étape)
1. Ouvrez **Présences → Ajouter la présence**.
2. Sélectionnez **la même Classe / Section** et **la même Date** que l'appel à corriger
   (+ le **même créneau** si l'appel initial était par cours).
3. La liste se recharge **avec les positions déjà enregistrées** : le pointage existant
   s'affiche.
4. Modifiez uniquement la/les ligne(s) fautive(s) (ex. remettre « present » un élève
   finalement venu l'après-midi).
5. **Soumettre**.
> Le système **met à jour** la fiche de présence de cet élève pour ce jour-là (il n'ajoute
> pas un doublon : une seule ligne par élève / classe / date / créneau). La correction est
> immédiate et remplace l'ancienne valeur.

## 🔁 Justifier une absence signalée à tort (SMS déjà parti)
- Le SMS au parent est **envoyé au moment du pointage** et ne se « rappelle » pas.
- Corrigez le pointage (ci-dessus), puis **appelez/messagez le parent** pour l'informer de
  la correction. Ne re-sélectionnez **pas** la case de notification si vous ne voulez pas
  qu'un second SMS parte.

## 🔴 « Annuler » un appel fait par erreur
Il n'existe **ni poubelle ni corbeille** pour les présences : un pointage ne se supprime pas
isolément. Selon le cas :
- **Appel enregistré pour un jour de fermeture** : repointez la même classe/date en cochant
  **« holiday »** → la journée devient un jour férié (comptée comme telle, plus d'« absent »).
- **Tous les élèves pointés absents par erreur** : repointez la date et remettez tout le
  monde « present » (ou le bon statut), puis **Soumettre**.
- **Un seul élève à retirer du compteur du jour** : repointez sa ligne à la bonne valeur.

## ♻️ Restaurer un pointage écrasé à tort
Il n'y a **pas d'historique ni de restauration** d'un pointage : la dernière soumission
gagne. Si vous avez écrasé un bon appel par erreur, **repointez la date une nouvelle fois**
avec les bonnes valeurs (en vous appuyant sur votre carnet/cahier papier ou sur la vue
mensuelle si elle n'était pas encore faussée). Faites toute correction **le plus tôt
possible**, avant que les totaux n'aient servis à d'autres calculs.

## ⚠️ Bon à savoir
- **La date est plafonnée à aujourd'hui** : on ne peut pas pointer le futur ; on peut
  toujours re-pointer une date **passée** de la session en cours.
- **Ne changez pas de créneau par erreur** : un appel « journée » (sans créneau) et un appel
  « par cours » sont des lignes **distinctes** (classe/élève/date/créneau). Pour corriger,
  reprenez exactement le même contexte.
- Les **retards** déclenchent parfois un SMS spécifique aux parents : vérifiez le statut
  (present/absent/retard) avant de valider.
- En cas de doute sur ce qui a été pointé, consultez d'abord **Présences → Consulter**
  (*02-consulter-presences.md*) **avant** de corriger.
