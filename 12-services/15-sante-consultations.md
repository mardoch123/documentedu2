---
id: 12-15-sante-consultations
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-15-sante-consultations
emoji: "🩺"
titre: "Santé : consultations et dossiers médicaux"
resume: "Le module Santé tient la santé de chaque élève : un dossier médical individuel (allergies, antécédents, groupe sanguin, contact d'urgence) et un journal de consultations (visites à l'infirmerie, mo..."
audiences: [school_admin, staff]
---
# 🩺 Santé : consultations et dossiers médicaux

## 🎯 Rôle
Le module **Santé** tient la **santé de chaque élève** : un **dossier médical** individuel
(allergies, antécédents, groupe sanguin, contact d'urgence) et un **journal de
consultations** (visites à l'infirmerie, motifs, constats, gestes). C'est l'outil de
l'**infirmier(ère) / du service santé** pour **suivre** et **retrouver** l'historique médical
d'un enfant.

## ✅ Prérequis
1. Option « **Health / Medical** » + permissions santé.
2. Avoir des **élèves** enregistrés.
3. Accès : menu **Health → Dashboard** (`health.dashboard`), **Dossiers**
   (`health.students.index`), **Consultations** (`health.consultations.index`).

## 🗂️ Le dossier médical d'un élève
1. Ouvrez **Dossiers médicaux / Students** (`health.students.index`).
2. **Recherchez l'élève**, ouvrez son **dossier** (`health.students.record`) :
   informations médicales de base, **allergies**, **antécédents**, **consultations passées**.
3. **Imprimer / exporter** le dossier en **PDF** (`health.students.record.pdf`) — utile pour
   une **urgence** ou un **médecin externe**.

## 🟢 Enregistrer une consultation (étape par étape)
1. Ouvrez **Consultations** → **« Nouvelle consultation »** (`health.consultations.create`,
   un élève peut être **pré-sélectionné**).
2. Renseignez : **élève**, **date/heure**, **motif**, **constats / symptômes**,
   **poids/taille/température** éventuels, **geste / traitement** administré, **observations**.
3. **Enregistrez** (`health.consultations.store`) : la consultation est **ajoutée au dossier**
   de l'élève.
4. **Consulter** une fiche : `health.consultations.show`.

## 📊 Tableau de bord santé
- `health.dashboard` : vue d'ensemble (**accès rapides** : nouvelle consultation, dossiers,
  ordonnance, examen, délivrer un médicament, statistiques) et **indicateurs** du service.

## ✏️ Modifier une fiche médicale
- Pour corriger un **dossier** (allergie mal saisie), rouvrez la fiche de l'élève et mettez-la
  à jour ; les **consultations** déjà enregistrées restent comme **journal** (trace des soins
  donnés à une date donnée).

## 🔴 Supprimer / ♻️ Restaurer
- ⚠️ Le **dossier médical** et les **consultations** sont un **document de soin** : ils ne
  partent **pas à la corbeille**. On ne **supprime** pas une consultation (intégrité
  médicale) ; une erreur se **corrige par une nouvelle note** ou en **éditant la fiche**
  concernée.
- La **radiation d'un élève** (PARTIE Élèves / Vie scolaire) archive son dossier avec lui.

## ⚠️ Bon à savoir
- **Confidentialité** : le dossier médical est **sensible** ; seules les personnes habilitées
  (service santé, direction) y accèdent.
- **Allergies & contacts d'urgence** : à **tenir absolument à jour** en tête de dossier
  (sécurité de l'enfant).
- **Le PDF du dossier** se remet au **parent/médecin** en cas de besoin.
- Les **ordonnances** prescrites ici alimentent la **pharmacie** (délivrance) — voir *16* et
  *17*.
- Les **statistiques santé** (maladies fréquentes, absences pour raison médicale) aident à la
  **médecine préventive** — voir *17*.
