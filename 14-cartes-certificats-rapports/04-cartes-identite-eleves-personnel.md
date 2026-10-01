---
id: 14-04-cartes-identite-eleves-personnel
partie: 14
titre_partie: "Cartes, certificats & rapports"
app: web
slug: 14-04-cartes-identite-eleves-personnel
emoji: "🪪"
titre: "Cartes d'identité élèves & personnel (impression interne)"
resume: "En plus de la commande de cartes plastifiées (01), l'école peut générer elle-même ses cartes d'identité au format PDF/image : paramétrer une fois le format de la carte (couleurs,"
audiences: [school_admin, staff]
---
# 🪪 Cartes d'identité élèves & personnel (impression interne)

## 🎯 Rôle
En plus de la **commande de cartes plastifiées** (*01*), l'école peut **générer elle-même**
ses **cartes d'identité** au format PDF/image : paramétrer une fois le **format de la carte**
(couleurs, textes, logos, dimensions) puis **générer les cartes** de tous les **élèves** ou de
tout le **personnel**, à imprimer sur carte blanche ou papier plastique.

## ✅ Prérequis
1. **Photos** des élèves/personnel présentes dans le système.
2. Être **School Admin**. Accès :
   - **Paramètres** → **ID Card Settings** (`id-card-settings`) ;
   - **Élèves** → **Generate ID Card** (`students.generate-id-card-index`) ;
   - **Personnel** → **ID Card** (`staff.id-card`) / **ID Card List** (`staff.show.all`).

## 🟢 Configurer le format de carte (une seule fois)
1. Ouvrez **Paramètres → ID Card Settings**.
2. Réglez : **texte/titre** de la carte, **couleurs**, **logo** de l'école, **éléments** à
   faire apparaître (nom, classe, matricule, année, groupe sanguin…).
3. **Enregistrez** (`POST id-card-settings`). Pour **retirer une image** déjà chargée :
   `id-card/remove/{type}`.

## 🟢 Générer les cartes des élèves (étape par étape)
1. Ouvrez **Élèves → Generate ID Card**.
2. Filtrez par **classe/section**, cochez les **élèves** concernés.
3. Lancez la **génération** (`students.generate-id-card`) → un **PDF des cartes** s'ouvre :
   imprimez-le (découpe après impression).

## 🟢 Générer les cartes du personnel
1. Ouvrez **Staff → ID Card** : carte individuelle d'un membre ;
   **ID Card List** (`staff.show.all`) : liste complète.
2. **Génération** (`POST staff/generate-id-card`) → PDF à imprimer.

## ✏️ Modifier
- Changez le **format** à tout moment dans **ID Card Settings** : les **générations
  suivantes** intègrent le nouveau design (les PDF déjà imprimés ne changent pas).
- Pour un **élève sans photo** : ajoutez la photo via sa fiche (*module Élèves*), puis
  régénérez.

## 🔴 Supprimer / ♻️ Restaurer
- Il n'y a **rien à supprimer** ici : la carte est un **document généré**, pas une donnée
  enregistrée. **Erreur de génération** → **régénérez** simplement après correction du
  paramétrage.
- ⚠️ Les **paramètres** de carte se **corrigeent** (Modifier), ne se suppriment pas.

## ⚠️ Bon à savoir
- **Différence claire** : *01* = cartes **plastifiées professionnelles** commandées et payées
  à la plateforme ; *ici* = cartes **imprimées par l'école** elle-même (coût = papier).
- **Règle d'impression** : utilisez du **cartonné** ; vérifiez l'**alignement** avec une
  feuille blanche avant la pleine production.
- **Recto seul** : ces impressions internes n'offrent pas de verso plastifié — pour un rendu
  officiel, préférez la **commande** (*01*).
- **Matricule** : assurez-vous que les **identifiants** sont bien générés
  (*Paramètres → Format des identifiants*).
