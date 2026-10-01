---
id: 15-17-gestion-site-web
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-17-gestion-site-web
emoji: "🌐"
titre: "Site web de l'école : contenu, modèles, aperçu, FAQ"
resume: "Chaque école EduEasy dispose d'un mini-site public (/ecole/...) que les parents visitent avant de s'inscrire."
audiences: [school_admin]
---
# 🌐 Site web de l'école : contenu, modèles, aperçu, FAQ

## 🎯 Rôle
Chaque école EduEasy dispose d'un **mini-site public** (`/ecole/...`) que les parents
visitent avant de s'inscrire. Ce module le **pilote** : choisir un **modèle (template) de
site**, remplir les **sections d'accueil** (présentation, points forts, services — avec
**ordre d'affichage**), gérer la **FAQ** (questions/réponses fréquentes) et **prévisualiser**
le résultat avant publication. C'est votre **vitrine en ligne**, sans webmaster.

## ✅ Prérequis
1. Être **School Admin** avec la fonction abonnement **« Website Management »**.
2. Avoir préparé **textes de présentation + photos** (logo, classes, activités).
3. Accès : **Paramètres → Web Settings / Site web** (`school.web-settings.index`).

## 🟢 Choisir un modèle de site (étape par étape)
1. Ouvrez la galerie des **templates de site** (`school.templates.website` /
   `templates.website`).
2. Parcourez les **modèles** ; cliquez sur celui qui vous plaît →
   **Sélectionner** (`school.templates.select-website`).
3. Le site prend immédiatement la **mise en page** du modèle (votre contenu suit).

## 🟢 Meubler les sections d'accueil (étape par étape)
1. Dans **Web Settings**, complétez le **contenu général** (titre accrocheur, description,
   services) → **Enregistrer** (`school.web-settings.store`).
2. **Sections à la carte** : ajoutez des **blocs** (`web-settings.feature.sections` →
   `.store`) : titre, texte, icône/image de chaque **point fort**.
3. **Modifier** un bloc : `web-settings-section.edit/{id}` → `update` ; les **monter/descendre**
   dans la page via le **changement d'ordre** (`feature_section_rank`).
4. **Supprimer** un bloc inutile : `web-settings-section.destroy/{id}` (⚠️ définitif :
   recréez-le pour le « restaurer »).

## ❓ Gérer la FAQ
1. Ouvrez la **FAQ** (`faqs.index`) : liste des questions posées par les parents.
2. **Ajouter** une question/réponse (`faqs.store`), **Modifier** (`faqs.update`),
   **Supprimer** (`faqs.destroy` — sans corbeille, recréez si besoin).

## 👁️ Prévisualiser
- Bouton **Aperçu** (`school.web-settings.preview` / `/school/website/preview`) : ouvre le
  site **tel que les parents le verront** — testez-le aussi sur **téléphone**.

## ⚠️ Bon à savoir
- **Photos nettes et légères** : la vitesse d'ouverture décide du départ des parents.
- **Un message clair en tête** : « École X — inscriptions 2026-2027 ouvertes au 15 août » :
  l'info que le parent cherche en 3 secondes.
- **Changer de modèle ne casse pas le contenu** : vous pouvez expérimenter librement.
- Les **pages légales** (contact, à propos…) se remplissent dans *12-pages-legales.md* et
  alimentent le même site.
- **La FAQ réduit les appels** : mettez-y les vraies questions du secrétariat (âges d'admission,
  uniformes, horaires, cantine).
