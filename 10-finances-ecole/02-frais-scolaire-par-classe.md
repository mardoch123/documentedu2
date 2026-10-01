---
id: 10-02-frais-scolaire-par-classe
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-02-frais-scolaire-par-classe
emoji: "💰"
titre: "Gérer une grille de frais par classe (Manage Fee)"
resume: "La « grille de frais » (Manage Fee) applique une tarification à une ou plusieurs classes : droits d'inscription, scolarité, frais obligatoires, facilités de paiement en tranches et prestations opti..."
audiences: [school_admin, staff]
---
# 💰 Gérer une grille de frais par classe (Manage Fee)

## 🎯 Rôle
La **« grille de frais »** (Manage Fee) applique une **tarification à une ou plusieurs
classes** : droits d'inscription, scolarité, frais obligatoires, **facilités de paiement en
tranches** et **prestations optionnelles**. C'est elle qui **génère les montants à payer** de
chaque élève des classes concernées. Une fois la grille créée, on peut **encaisser** les
paiements (*03*).

## ✅ Prérequis
1. Avoir **créé les types de frais** (*01-types-de-frais.md*).
2. Avoir **classes/sections** et une **année scolaire active**.
3. Permission « fees-list ». Accès : menu **Fees → Manage Fee** (`fees.index`).

## 🟢 Créer une grille de frais (3 étapes)
Le formulaire se déroule en **3 étapes** numérotées.

**Étape 1 — Libellé & classes ciblées**
1. **« Prefix Name »** ★ : le préfixe du nom (ex. « Scolarité 2026-2027 »). Le logiciel
   **combine préfixe + nom de classe** → « Scolarité 2026-2027 - 6ème A ». Utilisez
   **« Auto-générer »** ou un **modèle** rapide (Scolarité / Inscription / Frais Scolaires),
   et regardez l'**Aperçu** en direct.
2. **« Classes Concernées »** ★ : sélectionnez **une ou plusieurs classes** (« Tout
   sélectionner » / « Désélectionner »). Le compteur indique « N classe(s) sélectionnée(s) ».

**Étape 2 — Frais obligatoires de base**
3. Ajoutez **une ligne par frais obligatoire** (bouton d'ajout du repeater) :
   - **« Type de frais »** ★ (vos types créés ; + pour en créer un nouveau sans quitter) ;
   - **« Nouveaux élèves »** ★ — montant en **FCFA** (obligatoire) ;
   - **« Anciens élèves »** — montant (optionnel) s'il diffère ;
   - case **« Quantité »** si le montant dépend d'une quantité (ex. nb de mois) ;
   - **« date d'échéance »** ★ (date à partir de laquelle le frais est dû).
   > Le **« Total des frais obligatoires »** se met à jour en direct (en FCFA).

**Étape 3 — Facilités de paiement & tranches**
4. Choisissez la carte **« Paiement en une fois »** (désactivé tranches) ou
   **« Paiement échelonné »** (activé).
5. Si échelonné : ajoutez **une ligne par tranche** (nom, montant, date d'échéance). La somme
   des tranches doit correspondre au total (message de validation affiché).
6. Ajoutez éventuellement des **prestations optionnelles** (cantine, transport…) en repeater.
7. Cliquez **« Enregistrer la grille de frais »**.
8. La grille apparaît dans **« Grilles de Frais Actives »** et **facture automatiquement**
   les élèves des classes concernées.

## ✏️ Modifier une grille
1. Sur la ligne de la grille, cliquez l'**icône Modifier** (ouvre la page d'édition de la
   grille).
2. Ajustez libellé, classes, montants, tranches ou optionnels.
3. **Enregistrez**. (Modifier une grille déjà partiellement payée : prudent, les reçus
   existants restent.)

## 🔴 Supprimer une grille (corbeille)
1. Sur la ligne, cliquez **Supprimer** puis confirmez.
2. La grille part à la **corbeille** ; utilisez **« bulk-destroy »** pour en supprimer
   plusieurs d'un coup (cases à cocher).
3. Basculez **« all | Trashed »** sur **« Trashed »** pour voir les grilles supprimées.
4. Depuis « Trashed », la **suppression définitive** efface pour de bon.

## ♻️ Restaurer une grille supprimée
1. Liste en mode **« Trashed »**.
2. Cliquez **Restaurer** sur la grille voulue : elle **revient active** avec ses montants et
   tranches.

## ⚠️ Bon à savoir
- **Le total d'un frais est calculé depuis la grille par classe** : si les montants ne sont
  pas saisis dans la grille, l'élève verra « **0 FCFA** ». Renseignez toujours les montants.
- **Nouveaux vs Anciens élèves** : deux tarifs possibles pour le même frais (ex. droits
  d'inscription différents).
- **Dates d'échéance** : elles pilotent les **relances** et les **renvois pour impayés**
  (menu Fees → Renvois pour impayés, *voir Vie scolaire*).
- La grille crée **une entrée par classe sélectionnée** : 5 classes = 5 grilles au même
  préfixe.
- Le bouton **« Frais encaissés & purge »** mène au suivi des paiements (*03*).
- Pour paramétrer des règles globales (paiement séquentiel, reçus IA), voir
  **Fees Config** (`fees.config.index`).
