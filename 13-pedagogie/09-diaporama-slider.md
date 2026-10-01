---
id: 13-09-diaporama-slider
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-09-diaporama-slider
emoji: "🎞️"
titre: "Diaporama / Sliders (bannière de l'école)"
resume: "Le diaporama (sliders) alimente la bannière d'images défilantes affichée sur la page d'accueil du site de l'école (et parfois le tableau de bord)."
audiences: [school_admin]
---
# 🎞️ Diaporama / Sliders (bannière de l'école)

## 🎯 Rôle
Le **diaporama (sliders)** alimente la **bannière d'images défilantes** affichée sur la **page
d'accueil du site de l'école** (et parfois le tableau de bord). Vous y déposez des **images**
accompagnées d'un **titre** et d'un **lien** cliquable : c'est la **vitrine visuelle** de
l'établissement (photos d'événements, communications, promotions).

## ✅ Prérequis
1. Abonnement avec la fonction **« Slider Management »** activée.
2. Permission « slider-create ». Accès : menu **Sliders** (`sliders.index`).
3. Avoir des **images prêtes** (JPEG/PNG), de **format large/horizontal** pour la bannière.

## 🟢 Ajouter une image au diaporama (étape par étape)
1. Ouvrez **Sliders** → **« Ajouter »**.
2. Renseignez :
   - le **titre / légende** de l'image ;
   - le **lien** (URL) à ouvrir au clic (facultatif) ;
   - l'**image** elle-même (téléversement du fichier) ;
   - éventuellement un **ordre / statut** (affiché ou non).
3. **Enregistrez** (`sliders.store`). L'image rejoint la **rotation du bandeau**.

## ✏️ Modifier une image
1. Icône **Modifier** (`sliders.edit`) → changez titre/lien/image → `sliders.update`.
2. Pour **remplacer uniquement l'image**, re-téléversez le nouveau fichier dans le formulaire.

## 🔴 Supprimer une image
1. Icône **Supprimer** (`sliders.destroy`), confirmez → l'image **disparaît du bandeau**.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** : une image supprimée se **recrée** en la **re-téléversant** via
  « Ajouter ». Gardez vos **fichiers sources** de côté pour pouvoir les remettre.

## ⚠️ Bon à savoir
- **Format horizontal** : privilégiez des images **larges** (bannière) pour un rendu net.
- **Poids raisonnable** : des images trop lourdes **ralentissent** le site ; compressez-les.
- **3 à 5 images maximum** : trop de slides donne un effet « jukebox » ; gardez l'essentiel.
- **Lien cliquable** : renvoyez vers une **actualité**, une **inscription** ou un **événement**.
- La **Galerie** (*10-galerie.md*) est **différente** : le diaporama est la **bannière
  défilante**, la galerie est un **album photo** complet.
