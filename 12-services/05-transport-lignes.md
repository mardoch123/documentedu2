---
id: 12-05-transport-lignes
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-05-transport-lignes
emoji: "🛣️"
titre: "Transport : lignes de transport (+ affectation d'un élève)"
resume: "Une ligne (Route) relie une suite d'arrêts (04) dans un ordre de passage défini, et porte une tarification par élève."
audiences: [school_admin, staff]
---
# 🛣️ Transport : lignes de transport (+ affectation d'un élève)

## 🎯 Rôle
Une **ligne (Route)** relie une **suite d'arrêts** (*04*) dans un **ordre de passage**
défini, et porte une **tarification** par élève. C'est l'**épine dorsale** du transport : un
élève est **affecté à une ligne + un arrêt**, ce qui génère son **frais de transport**. Cette
page couvre la **création des lignes**, l'**ordre des arrêts**, les **frais**, et
l'**affectation d'un élève via une demande de transport**.

## ✅ Prérequis
1. Avoir créé les **arrêts** (*04*) et les **véhicules** (*03*).
2. Option « **Transport Management** » + permissions routes.
3. Accès : menu **Transport → Routes** (`routes.index`) et **Transportation Requests**
   (`transportation-requests`).

## 🟢 Créer une ligne (étape par étape)
1. Ouvrez **Routes**, cliquez **« Ajouter »** (`routes.create`).
2. Renseignez : **nom de la ligne**, les **arrêts** qui la composent, et les **frais**
   associés.
3. **Enregistrez** (`routes.store`). La ligne apparaît dans la liste.

## 🔢 Ordonner les arrêts d'une ligne
1. Sur la ligne, ouvrez **« Changer l'ordre »** (`routes.change-order`).
2. **Réorganisez les arrêts** dans l'ordre réel de passage, puis validez
   (`routes.update-pickup-order`, PUT).
3. Pour **ôter un arrêt** de la ligne : `pickup-points.delete`.

## 💵 Régler les frais de la ligne
- Les **frais de transport** d'une ligne se **modifient** ici :
  `transportation-fees.edit` → `transportation-fees.update` (montant par élève/arrêt).
- **Supprimer un frais** : `transportation-fees.destroy`.

## 🧑‍🎓 Affecter un élève à une ligne (demande de transport)
1. Ouvrez **Transportation Requests** (`transportation-requests.index`).
2. **Recherchez l'élève** (`search-students`) — ou passez par une **saisie hors-ligne**
   (`transportation-requests.offline-entry` → `offline-entry.store`) si le parent n'a pas
   l'app.
3. Choisissez la **ligne / le véhicule** (`get-vehicle-routes` selon l'arrêt), l'**arrêt** de
   montée.
4. **Validez la demande** : l'élève est **transporté** sur cette ligne et le **frais de
   transport** est généré ; un **reçu** est disponible (`transportation-requests.fee-receipt`).
5. **Changement de statut en masse** : cases à cocher + `change-status-bulk`.

## ✏️ Modifier / 🔴 Supprimer une ligne
- **Modifier** : `routes.edit` → `routes.update` (nom, arrêts, frais).
- **Supprimer** : icône **Supprimer** (`routes.destroy`), confirmez.

## ♻️ Restaurer
- ⚠️ Les **lignes ne sont pas restaurables** (pas de corbeille) : une ligne supprimée se
  **recrée** et se **ré-ordonne** ; les **affectations d'élèves** perdues doivent être
  **refaites** via les demandes de transport. **Ne supprimez donc pas une ligne active** :
  contentez-vous de la vider de ses arrêts/élèves.
- Une **affectation d'élève** se **retrait** proprement par
  `transportation-requests.cancel` (annulation du service), **sans supprimer la ligne**.

## ⚠️ Bon à savoir
- **Ordre des arrêts = parcours réel** : un mauvais ordre embrouille chauffeur et parents.
- **Un élève = une ligne + un arrêt** ; changer d'arrêt = nouvelle demande / annulation
  (cancel) puis recréation.
- **Reçu de transport** (`fee-receipt`) : justificatif du paiement du frais.
- La **demande hors-ligne** (`offline-entry`) est utile quand le parent ne peut pas passer
  par l'application : la caisse saisit pour lui.
- Les **véhicules** sont **associés à la ligne** dans *06-transport-camions-lignes.md* ; les
  **recettes/dépenses** de transport suivent dans *08*.
