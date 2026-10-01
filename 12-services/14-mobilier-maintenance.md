---
id: 12-14-mobilier-maintenance
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-14-mobilier-maintenance
emoji: "🛠️"
titre: "Mobilier : demandes et suivi de maintenance"
resume: "La maintenance gère la vie technique du matériel : déclarer une panne/casse, assigner une réparation, suivre l'avancement et clôturer quand le bien est rétabli."
audiences: [school_admin, staff]
---
# 🛠️ Mobilier : demandes et suivi de maintenance

## 🎯 Rôle
La **maintenance** gère la **vie technique** du matériel : **déclarer une panne/casse**,
**assigner une réparation**, suivre l'**avancement** et **clôturer** quand le bien est rétabli.
Elle ajoute la **maintenance préventive** (entretiens planifiés pour **éviter** les pannes).
Le **bon suivi** prolonge la durée de vie du mobilier et maîtrise les coûts.

## ✅ Prérequis
1. Avoir un **catalogue** de biens (*12*).
2. Permission « furniture-maintenance-list » (déclaration) / gestion maintenance.
3. Accès : menu **Furniture → Maintenance** (`furniture.maintenance.index`).

## 🟢 Déclarer une panne (étape par étape)
1. Ouvrez **Maintenance** ; cliquez **« Signaler »** / déclaration rapide
   (`furniture.maintenance.report-quick`) — ou **scannez le QR du bien** (*12*).
2. Renseignez : le **bien** concerné, la **description de la panne**, la **gravité**,
   éventuellement une **photo**.
3. **Envoyez** : une **demande de maintenance** est créée ; le bien bascule en
   **« en réparation »** (visible au compteur *12*).

## 👷 Assigner puis clôturer une réparation
1. Ouvrez la **demande** (`furniture.maintenance.show`) : son détail et son statut.
2. **Assignez** un réparateur / une action (`furniture.maintenance.assign`).
3. Une fois la réparation **faite**, **clôturez** la demande (`furniture.maintenance.close`) :
   le bien **redevient « en service »**.

## 📅 Maintenance préventive
1. Ouvrez **Preventive** (`furniture.maintenance.preventive`).
2. **Planifiez** un entretien (ex. « révision trimestrielle des bureaux », « vérification des
   extincteurs ») : `furniture.maintenance.preventive.store`.
3. Ces **RD d'entretien** aident à **prévenir** les pannes plutôt qu'à les subir.

## 📋 Suivi
- **Liste des demandes** (`furniture.maintenance.list`) : filtrez par **statut** (ouverte, en
  cours, clôturée), par bien, par gravité.
- Les compteurs du **catalogue** (*12*) reflètent en direct le nombre de biens **« en
  réparation »** et **« hors service »**.

## ✏️ / 🔴 / ♻️ Corriger, annuler, restaurer
- Une demande se **complète** (assignation, clôture) plutôt qu'elle ne s'édite ; pour tout
  annuler, on **clôture** sans intervenir ou on **re-déclare** proprement.
- ⚠️ **Pas de corbeille** pour les maintenances : l'historique des réparations est **un
  journal** qu'on **ne supprime pas** (c'est la mémoire technique du matériel). Une erreur se
  **corrige par une nouvelle entrée**.

## ⚠️ Bon à savoir
- **Photo + gravité** aident le réparateur à intervenir **avec les bonnes pièces**.
- **Ne supprimez pas** un bien en panne : passez-le en **réparation/hors service** pour garder
  la **statistique de casse** (matériel fragile, fournisseur…).
- La **préventive planifiée** coûte moins cher que les **réparations d'urgence** : programmez-la.
- Une **casse irréparable** → le bien part **« hors service »** (*12*) et une **acquisition de
  remplacement** est à prévoir (hors périmètre de ce module).
- Lié au **mouvement** (*13*) : parfois un bien est **déplacé** le temps de la réparation.
