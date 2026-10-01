---
id: 12-03-transport-vehicules
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-03-transport-vehicules
emoji: "🚌"
titre: "Transport : véhicules (créer / supprimer / restaurer)"
resume: "Un véhicule est un bus, minibus ou camion affecté au transport scolaire."
audiences: [school_admin, staff]
---
# 🚌 Transport : véhicules (créer / supprimer / restaurer)

## 🎯 Rôle
Un **véhicule** est un **bus, minibus ou camion** affecté au transport scolaire. Cette page
tient le **parc automobile** de l'école : immatriculation, type, **capacité**, état. Les
véhicules sont ensuite **associés à des lignes** (*06*) et conduit par des **chauffeurs**
(*07*). Cycle complet pris en charge : **créer, modifier, supprimer (corbeille), restaurer**.

## ✅ Prérequis
1. Option « **Transport Management** » + permissions véhicule.
2. Accès : menu **Transport → Vehicles** (`vehicles.index`).

## 🟢 Créer un véhicule (étape par étape)
1. Ouvrez **Vehicles**, cliquez **« Ajouter »** (`vehicles.create`).
2. Renseignez la **fiche du véhicule** :
   - **Nom / désignation** (ex. « Bus 01 ») ;
   - **Immatriculation** ;
   - **Type** (bus, minibus, camion…) ;
   - **Capacité** (nombre de places) ;
   - toute info utile (état, assurance, observations).
3. **Enregistrez** (`vehicles.store`). Le véhicule apparaît dans la **liste du parc**
   (`vehicles.show`).

## ✏️ Modifier un véhicule
1. Icône **Modifier** sur la ligne (`vehicles.edit`).
2. Ajustez capacité, immatriculation, état… puis `vehicles.update`.

## 🔴 Supprimer un véhicule (corbeille)
1. Icône **Supprimer** sur la ligne (`vehicles.destroy`, route `vehicles/{id}/deleted`) puis
   **confirmez**.
2. Le véhicule part à la **corbeille** (soft delete) : il **disparaît** de la liste active
   mais reste **récupérable**.
3. Basculez **« all | Trashed »** sur **« Trashed »** pour voir les véhicules supprimés.
4. Depuis « Trashed », la **suppression définitive** (`vehicles.trash`,
   `vehicles/{id}/trash`) efface pour de bon.

## ♻️ Restaurer un véhicule supprimé
1. Liste en mode **« Trashed »**.
2. Cliquez **Restaurer** (`vehicles.restore`, `vehicles/{id}/restore`).
3. Le véhicule **revient dans le parc**, avec ses **affectations de lignes** conservées.

## ⚠️ Bon à savoir
- **Ne supprimez pas un véhicule encore affecté** à une ligne active : retirez d'abord
  l'association (*06*) pour ne pas casser le transport des élèves.
- **Capacité** : elle sert à **limiter le nombre d'élèves** par ligne/véhicule.
- Un véhicule **mal orthographié ou en double** se corrige par **Modifier** plutôt que
  supprimer/recréer (l'historique est conservé).
- **Corbeille = filet de sécurité** : toute suppression est réversible tant que vous n'avez
  pas vidé « Trashed ».
- Les **chauffeurs/aides** sont un **répertoire séparé** (*07*) qu'on **attache** au
  véhicule/ligne ; le véhicule lui-même n'est pas « connecté » à un compte utilisateur.
