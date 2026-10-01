---
id: 14-07-prospectus-fournitures-ia
partie: 14
titre_partie: "Cartes, certificats & rapports"
app: web
slug: 14-07-prospectus-fournitures-ia
emoji: "📕"
titre: "Prospectus & liste de fournitures (20 designs + IA)"
resume: "Ce module crée le prospectus de rentrée de l'école : un document joliment mis en page (au choix parmi 20 designs) présentant les informations pratiques et surtout la liste des fournitures scolaires..."
audiences: [school_admin, staff]
---
# 📕 Prospectus & liste de fournitures (20 designs + IA)

## 🎯 Rôle
Ce module crée le **prospectus de rentrée** de l'école : un **document joliment mis en page**
(au choix parmi **20 designs**) présentant les **informations pratiques** et surtout la
**liste des fournitures scolaires par classe**. L'**IA** peut **générer automatiquement** une
liste de fournitures **adaptée au niveau** de la classe ; vous **relisez, ajustez**,
**enregistrez** et **prévisualisez** avant diffusion aux parents.

## ✅ Prérequis
1. Être **School Admin** (module protégé, inaccessible aux enseignants).
2. Avoir vos **classes** créées (la liste de fournitures se rattache à une classe).
3. Accès : menu **Prospectus** (`prospectus.index`).

## 🟢 Créer un prospectus (étape par étape)
1. Ouvrez **Prospectus**.
2. Choisissez le **design** (parmi les **20 modèles**, ex. *modern-minimal*…).
3. Renseignez le **contenu** : textes d'accueil, dates de rentrée, coordonnées, informations
   aux parents.
4. **Enregistrez** (`prospectus.save`) puis **Prévisualisez** (`prospectus.preview`) pour
   voir le rendu exact.

## 🤖 Générer la liste de fournitures par IA (étape par étape)
1. Dans la section **Fournitures**, choisissez la **classe** (`class_name`, ex. *CP*) et
   l'éventuel **profil/filière** (`stream_name`).
2. Lancez la **génération IA** (`prospectus.generate-ai-supplies`) : l'IA propose la
   **liste des fournitures** du niveau (cahiers, crayons, géométrie, manuels…).
3. **Relisez et modifiez** les lignes (quantités, précision des articles).
4. **Enregistrez la liste** pour la classe (`prospectus.save-supplies`, avec `class_id`).
5. Répétez pour **chaque classe** ; la **prévisualisation** intègre les listes sauvegardées.

## ✏️ Modifier
- Retournez dans **Prospectus** : changez le **design**, les **textes** ou une **liste** de
  fournitures, puis **ré-enregistrez** (`prospectus.save` / `prospectus.save-supplies`).
- Le **prospectus** et les listes se **mettent à jour** sur place (un seul état par école).

## 🔴 Supprimer / ♻️ Restaurer
- ⚠️ **Pas de suppression** : le prospectus est un **document de travail continu** — on le
  **remplace** en éditant, on ne l'efface pas. Une liste de fournitures se **modifie**
  simplement avant enregistrement.

## ⚠️ Bon à savoir
- **L'IA propose, vous disposez** : vérifiez les **quantités** et le **programme local**
  (telle école exige telle marque de cahier) — ajustez toujours.
- **Un design sobre** se lit mieux par les parents ; privilégiez lisibilité > effets.
- **Diffusion** : exportez/photocopiez le prospectus après prévisualisation, ou partagez-le
  via les **annonces** aux parents.
- **Rentrée annuelle** : **refaites le prospectus chaque année** (dates et niveaux changent).
- La **prévisualisation** peut aussi être vue côté **site public de l'école** selon le
  paramétrage (`prospectus.preview` avec id d'école).
