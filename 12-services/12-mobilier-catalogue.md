---
id: 12-12-mobilier-catalogue
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-12-mobilier-catalogue
emoji: "🪑"
titre: "Mobilier : catalogue des biens (+ import, étiquettes QR)"
resume: "Le catalogue mobilier inventorie tout le patrimoine matériel de l'école : tables, chaises, bureaux, tableaux, ordinateurs, armoires…"
audiences: [school_admin, staff]
---
# 🪑 Mobilier : catalogue des biens (+ import, étiquettes QR)

## 🎯 Rôle
Le **catalogue mobilier** inventorie tout le **patrimoine matériel** de l'école : tables,
chaises, bureaux, tableaux, ordinateurs, armoires… Chaque **bien** porte une **référence**, un
**emplacement** (salle) et un **état** (en service, en réparation, hors service). On peut
**ajouter** des biens (à l'unité ou par **import**) et leur coller une **étiquette QR** pour
l'**inventaire physique**.

## ✅ Prérequis
1. Option « **Furniture Management** » + permissions mobilier.
2. Accès : menu **Furniture** (`furniture.index`), liste des biens (`furniture.items.list`).

## 🟢 Ajouter un bien (étape par étape)
1. Ouvrez **Furniture** ; le **tableau de bord** affiche les compteurs : **total, en
   réparation, hors service**.
2. **Ajout rapide** (`furniture.items.quick`) : **nom du bien**, **référence / code**,
   **catégorie**, **emplacement (salle)**, **quantité**, **état**.
3. **Enregistrez** : le bien rejoint le **catalogue**.

## ✏️ Consulter / modifier un bien
- **Fiche du bien** (`furniture.items.show`) : ses caractéristiques, son **historique**
  (mouvements *13*, maintenances *14*).
- **Modifier** (`furniture.items.update`, POST `furniture/items/{id}`) : changer emplacement,
  état, infos.

## 📥 Import en masse (Excel / CSV)
1. Menu **Furniture → Import** (`furniture.import.index`).
2. **Téléchargez le modèle**, remplissez une ligne par bien, **déposez** le fichier
   (dropzone), **Importez** (`furniture.import.upload`).
3. Idéal pour **saisir tout un inventaire** d'un coup.

## 🏷️ Étiquettes QR d'inventaire
1. Menu **Furniture → Labels** (`furniture.labels.index`).
2. **Sélectionnez** les biens, **imprimez** la planche (`furniture.labels.print`).
3. **Collez** chaque QR sur le bien : le **scan** permet de le **localiser / bouger /
   déclarer une panne** instantanément (*13* / *14*).

## 🔴 Retirer / restaurer un bien
- Le mobilier fonctionne par **état** : un bien **cassé** passe en **« en réparation »** ou
  **« hors service »** (vu aux compteurs) au lieu d'être supprimé — l'**inventaire reste
  cohérent**.
- ⚠️ **Pas de corbeille web « Trashed »** pour les biens : un bien **sorti** se **ré-intègre**
  en **remettant son état à « en service »** (`furniture.items.update`) ; un bien supprimé par
  erreur se **recrée** ou se **ré-importe** (CSV).

## ⚠️ Bon à savoir
- **Un QR par bien** (ou par lot identique) : le scan déclenche **mouvement** (*13*) ou
  **demande de maintenance** (*14*) en 3 clics.
- **Nommez les emplacements** clairement (salle 12, bureau direction…) : c'est la base du
  suivi des **mouvements**.
- **Référence unique** : évitez les doublons, elle sert de repère dans l'import et les QR.
- L'**état « hors service »** garde la **trace** du matériel réformé sans fausser les totaux.
- Suite logique : **Mouvements & affectations** (*13*) et **Maintenance** (*14*).
