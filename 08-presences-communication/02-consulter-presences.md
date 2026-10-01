---
id: 08-02-consulter-presences
partie: 8
titre_partie: "Présences & communication"
app: web
slug: 08-02-consulter-presences
emoji: "👁️"
titre: "Consulter les présences (journalière et mensuelle)"
resume: "Vérifier qui était là, quand : la consultation « journalière » affiche l'appel d'une date précise, la vue « mensuelle » montre un calendrier par jour du mois pour toute une classe"
audiences: [school_admin, teacher, staff]
---
# 👁️ Consulter les présences (journalière et mensuelle)

## 🎯 Rôle
Vérifier **qui était là, quand** : la consultation « journalière » affiche l'appel d'une date
précise, la vue « mensuelle » montre un **calendrier par jour du mois** pour toute une classe —
l'outil idéal pour repérer un élève qui s'absente souvent, justifier une statistique à un
parent, ou préparer un conseil de classe.

## ✅ Prérequis
1. Que des appels aient déjà été **pointés** (voir *01-pointage-presences-eleves.md*).
2. Permission « attendance-list » (ou « class-teacher » pour votre classe).
3. Option d'abonnement « Attendance Management ».
4. Accès : menu **Présences → Consulter la présence (view_attendance)** et
   **Présences → Vue mensuelle (month_wise)**.

## 🟢 Consulter un jour précis (étape par étape)
1. Ouvrez **Présences → Consulter la présence**.
2. Sélectionnez la **Classe / Section**.
3. Choisissez la **Date** (jours passés uniquement).
4. *(Filtre utile)* **Statut** : « Tous », **present**, **absent** ou **holiday** — pour
   n'afficher que les absents du jour par exemple.
5. *(Filtre utile)* **Séance / créneau** si l'appel a été fait par cours.
6. La liste s'affiche : chaque élève avec sa position du jour.
7. **Export 📤** : téléchargez la liste du jour (Excel/PDF) pour l'archiver ou la remettre
   à l'administration.

## 🗓️ Consulter le mois complet (étape par étape)
1. Ouvrez **Présences → Vue mensuelle**.
2. Sélectionnez la **Classe / Section**, puis le **Mois ★**.
3. Le tableau se construit **avec une colonne par jour du mois** (1…31) et une ligne
   par élève : position de chaque jour visible d'un coup (présent/absent/férié…).
4. Faites défiler horizontalement pour parcourir les jours du mois.
5. Un élève avec une **rayure d'absences qui se répète** (mêmes jours de la semaine, week-ends
   prolongés…) : c'est exactement ce signal qu'il faut surveiller → signalement vie scolaire
   ou module **décrochage IA**.

## ✏️ « Modifier » depuis la consultation
La consultation est en **lecture seule** : pour corriger une position, on repointe l'appel de
la date concernée → voir *03-modifier-supprimer-presence.md*.

## 🔴 / ♻️ Suppression et restauration
Aucune suppression ici (c'est un écran de lecture) ; les corrections passent par le
repointage. Voir *03-modifier-supprimer-presence.md* pour tout le cycle.

## ⚠️ Bon à savoir
- **Écart entre « Ajouter » et « Consulter »** : l'écran d'ajout sert à POINTER ; celui-ci sert
  à LIRE. Ne cherchez pas de boutons d'édition dans la consultation.
- La vue mensuelle est le **meilleur outil du conseil de classe** : imprimez-la (via le navigateur)
  pour avoir l'historique sous les yeux.
- Les totaux de la **page d'accueil / tableau de bord** (absents du jour) proviennent des
  mêmes pointages : en cas de doute, la vérité est dans cette consultation.
- Les élèves **transférés/désactivés** en cours de mois peuvent apparaître sans pointage après
  leur départ : normal.
