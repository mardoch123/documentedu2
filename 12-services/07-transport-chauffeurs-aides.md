---
id: 12-07-transport-chauffeurs-aides
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-07-transport-chauffeurs-aides
emoji: "🚍"
titre: "Transport : chauffeurs et aides (create / delete / restore)"
resume: "Les chauffeurs et aides (accompagneurs) sont le personnel de conduite du transport."
audiences: [school_admin, staff]
---
# 🚍 Transport : chauffeurs et aides (create / delete / restore)

## 🎯 Rôle
Les **chauffeurs** et **aides** (accompagneurs) sont le **personnel de conduite** du
transport. Cette page tient leur **répertoire** (identité, permis, rôle chauffeur/aide),
permet l'**import en masse** et l'**activation/désactivation**, et est reliée aux
**véhicules/lignes** (*06*). Cycle complet : **créer, modifier, supprimer (corbeille),
restaurer**.

## ✅ Prérequis
1. Option « **Transport Management** » + permissions driver-helper.
2. Accès : menu **Transport → Driver & Helper** (`driver-helper.index`).

## 🟢 Créer un chauffeur / une aide (étape par étape)
1. Ouvrez **Driver & Helper**, cliquez **« Ajouter »** (`driver-helper.create`).
2. Renseignez : **nom**, **prénom**, **téléphone**, **type** (**Chauffeur** ou **Aide**),
   **permis / pièces** (numéro, validité) et **statut** (actif/inactif).
3. **Enregistrez** (`driver-helper.store`). La personne apparaît au répertoire et peut être
   **affectée à un véhicule/ligne** (*06*).

## 📥 Import en masse (Bulk Upload)
1. Bouton **« Bulk upload »** (`driver-helper.create-bulk-upload`).
2. **Téléchargez le modèle** (`driver-helper.bulk-data-sample`) pour les **colonnes exactes**.
3. Remplissez le **CSV**, puis **Importez** (`driver-helper.store-bulk-upload`).

## ⏸️ Activer / désactiver
- **Au cas par cas** : `driver-helper/{id}/change-status` (restore/réactivation) — un aide
  indisponible est **désactivé** sans être supprimé.
- **En masse** : cases à cocher + `driver-helper/change-status-bulk`.

## ✏️ Modifier un chauffeur / une aide
1. Icône **Modifier** (`driver-helper.edit`) → corrigez identité, permis, type →
   `driver-helper.update`.

## 🔴 Supprimer (corbeille)
1. Icône **Supprimer** (`driver-helper.destroy`), confirmez.
2. L'entrée part à la **corbeille** ; basculez **« all | Trashed »** sur **« Trashed »**.
3. Depuis « Trashed », **suppression définitive** (`driver-helper.trash`).

## ♻️ Restaurer
1. Mode **« Trashed »**.
2. **Restaurer** (`driver-helper.restore`) → la personne **revient** dans le répertoire.

## ⚠️ Bon à savoir
- **Préférez désactiver à supprimer** : un chauffeur saisonnier ou momentanément absent se
  **désactive** (historique conservé), il ne se supprime pas.
- **Corbeille sécurisée** : suppression toujours réversible via « Trashed » + Restaurer.
- La **sécurité** passe par le **permis à jour** : notez **numéro et validité** du permis sur
  la fiche ; un permis expiré ne doit pas conduire.
- Un **chauffeur** peut être rattaché à un **compte de connexion** s'il doit pointer sa
  présence (QR/attendance) ; sinon c'est une **fiche administrative**.
- Ne pas confondre avec le **Staff** général (*PARTIE 11 — 04*) : les **chauffeurs/aides**
  ont **leur propre répertoire** transport (mais logique identique : import, statut, restore).
