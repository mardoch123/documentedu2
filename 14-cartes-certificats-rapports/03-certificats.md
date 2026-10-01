---
id: 14-03-certificats
partie: 14
titre_partie: "Cartes, certificats & rapports"
app: web
slug: 14-03-certificats
emoji: "🎓"
titre: "Certificats (élèves, personnel) et modèles"
resume: "Le module Certificats produit les documents officiels de l'école : certificat de scolarité, certificat de fin d'année, attestations pour élèves et pour le personnel."
audiences: [school_admin, staff]
---
# 🎓 Certificats (élèves, personnel) et modèles

## 🎯 Rôle
Le module **Certificats** produit les **documents officiels** de l'école : **certificat de
scolarité**, **certificat de fin d'année**, attestations pour **élèves** et pour le
**personnel**. Vous créez d'abord un **modèle** (mise en page + texte avec variables), puis
vous **génerez** le certificat pour une personne : le document s'affiche et
**s'imprime/s'exporte en PDF**.

## ✅ Prérequis
1. Avoir **élèves** et/ou **personnel** enregistrés, et le **nom de l'école** correctement
   paramétré (*Paramètres généraux*).
2. Permissions « certificate-* ». Accès : menu **Certificates**
   (`certificate-template.index`) + pages **Student Certificate** (`/certificate`) et
   **Staff Certificate** (`/certificate/staff-certificate`).

## 🟢 Créer un modèle de certificat (étape par étape)
1. Ouvrez **Certificate Templates** → **« Ajouter »** (`certificate-template.create`).
   Deux voies : le formulaire **classique** (`certificate-template.classic`) ou le
   **concepteur visuel** (`certificate-template.design/{id}` puis `PUT design/{id}`) pour
   placer textes, images et variables à la souris.
2. Renseignez : **titre du modèle**, **corps du texte** avec **variables** (nom de l'élève,
   classe, année, date…), **logo/signature**.
3. **Enregistrez** (`certificate-template.store`). Le modèle est réutilisable.
4. **Catalogue** : des modèles prêts à l'emploi peuvent être **installés** depuis le
   catalogue (`templates.certificate` → `templates.certificate.install`).

## 📄 Générer un certificat élève
1. Ouvrez la page **Student Certificate** (`/certificate`).
2. Choisissez le **modèle**, la **classe**, l'**élève**, les informations demandées.
3. **Générer** (`POST /certificate`) → le certificat s'affiche : **imprimez** (Ctrl+P) ou
   exportez en **PDF**.

## 📄 Générer un certificat personnel (staff)
1. Ouvrez **Staff Certificate** (`/certificate/staff-certificate`).
2. Choisissez le **modèle** et le **membre du personnel** → **Générer**
   (`POST staff-certificate`) → **PDF/impression**.

## ✏️ Modifier un modèle
1. Icône **Modifier** (`certificate-template.edit`) → ajustez texte/variables/mise en page →
   `certificate-template.update`. Les **générations futures** utiliseront le nouveau texte ;
   les PDF déjà imprimés ne changent pas.

## 🔴 Supprimer un modèle
1. Icône **Supprimer** (`certificate-template.destroy`), confirmez → le modèle **disparaît**.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** : un modèle supprimé est **définitivement perdu** (les certificats
  déjà imprimés restent-valides hors du système). **Recréez** le modèle, ou **réinstallez-le**
  depuis le **catalogue** si c'était un modèle standard.

## ⚠️ Bon à savoir
- **Variables = automatisme** : laissez le système remplir nom/classe/date via les
  variables ; ne les tapez pas « en dur » dans le modèle.
- **Génération ≠ stockage** : le certificat existe au moment de l'impression ; **archivatez**
  les PDF importants dans votre ordinateur.
- **Un modèle par usage** : créez des modèles distincts « Scolarité » / « Fin d'année » /
  « Personnel » pour ne pas vous tromper.
- Cartes d'identité : autre module, voir *04-cartes-identite-eleves-personnel.md*.
