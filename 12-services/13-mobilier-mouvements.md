---
id: 12-13-mobilier-mouvements
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-13-mobilier-mouvements
emoji: "🔄"
titre: "Mobilier : mouvements, vue par salle et affectation"
resume: "Un mouvement trace chaque déplacement d'un bien d'une salle à une autre (affectation, transfert) et sa réception."
audiences: [school_admin, staff]
---
# 🔄 Mobilier : mouvements, vue par salle et affectation

## 🎯 Rôle
Un **mouvement** trace chaque **déplacement d'un bien** d'une **salle à une autre**
(affectation, transfert) et sa **réception**. La **vue par salle** montre **ce qui se trouve
dans chaque pièce** ; l'**affectation en 3 clics** permet de **poser un bien dans une salle**
rapidement (au besoin par **scan QR**). Chaque mouvement peut s'**imprimer en PDF** (bordereau
signé).

## ✅ Prérequis
1. Avoir un **catalogue** de biens et des **salles/emplacements** (*12*).
2. Permission « furniture-movement-list » (et assignation).
3. Accès : menu **Furniture → Movements** (`furniture.movements.index`) et
   **Furniture → Rooms** (`furniture.movements.rooms`).

## 🏫 Vue par salle
1. Ouvrez **Rooms** (`furniture.movements.rooms`) : la **liste des pièces**.
2. Cliquez une **salle** pour voir **tout le mobilier qui s'y trouve** (et son état).

## 🟢 Affecter un bien à une salle (3 clics)
1. Ouvrez **Assign** (`furniture.movements.assign`).
2. **Choisissez le bien** (sélection ou **scan de son QR** *12*), **la salle de destination**,
   validez (`furniture.movements.assign.store`).
3. Le **mouvement** est créé : le bien est désormais **localisé** dans cette salle.

## ↔️ Transférer un bien d'une salle à l'autre
- **Transfert direct** (`furniture.movements.transfer-item`) : le bien change d'emplacement en
  une opération (l'ancien et le nouveau sont tracés).

## ✅ Réceptionner un mouvement
1. Quand un bien est envoyé quelque part, le destinataire **réceptionne** :
   `furniture.movements.receive.form` (formulaire) → `furniture.movements.receive.store`.
2. La **réception** (avec **signature** éventuelle) **clôt** le mouvement et **confirme** la
   nouvelle localisation.

## 🖨️ Imprimer le bordereau
- Chaque mouvement s'**imprime en PDF** (`furniture.movements.pdf/{id}`) : **bordereau de
  transfert / décharge** à faire **signer** (traçabilité du matériel qui bouge).

## 📋 Historique des mouvements
- **Liste** (`furniture.movements.list`) : tous les déplacements (qui, quoi, d'où → où, quand,
  statut : en cours / réceptionné).

## ✏️ / 🔴 / ♻️ Corriger, annuler, restaurer
- Un mouvement est un **événement du journal** : on ne l'**édite** pas, on crée un **nouveau
  mouvement** pour **ramener** le bien là où il devait être (mouvement correctif).
- ⚠️ **Pas de corbeille** pour les mouvements : ils **s'annulent par l'action inverse**
  (re-transfert / réception), l'historique restant **intègre**.

## ⚠️ Bon à savoir
- **Scannez l'étiquette QR** (*12*) pour affecter/transférer **sans erreur de saisie**.
- **Faites réceptionner** systématiquement : un mouvement non réceptionné = matériel « en
  route » (localisation incertaine).
- Le **bordereau PDF signé** est votre **preuve** en cas de perte/déplacement non autorisé.
- La **vue par salle** sert lors des **inventaires physiques** et des **rentrées** (vérifier
  que chaque classe a son mobilier).
- Les **pannes** déclarées sur un bien basculent son **état** et ouvrent une **maintenance**
  (*14*).
