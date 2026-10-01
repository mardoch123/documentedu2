---
id: 13-10-galerie
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-10-galerie
emoji: "🖼️"
titre: "Galerie photos de l'école (School Gallery)"
resume: "La galerie est l'album photo de l'établissement : on y dépose des images (et parfois des vidéos/fichiers) par événement — rentrée, sortie scolaire, remise de prix, sports, fête…"
audiences: [school_admin]
---
# 🖼️ Galerie photos de l'école (School Gallery)

## 🎯 Rôle
La **galerie** est l'**album photo** de l'établissement : on y dépose des **images** (et parfois
des **vidéos/fichiers**) par **événement** — rentrée, sortie scolaire, remise de prix,
sports, fête… Chaque **dépôt** (gallery entry) regroupe un **titre**, une **description** et
un ou plusieurs **fichiers**. C'est la **mémoire visuelle** partagée avec les parents et le
site de l'école.

## ✅ Prérequis
1. Abonnement avec la fonction **« School Gallery Management »** activée.
2. Permissions « gallery-* ». Accès : menu **Gallery** (`gallery.index`).
3. Avoir vos **photos prêtes** (JPEG/PNG, ou vidéo selon le champ proposé).

## 🟢 Ajouter une galerie / des photos (étape par étape)
1. Ouvrez **Gallery** → **« Ajouter »**.
2. Renseignez :
   - le **titre** de l'album / de l'événement (ex. : *Sortie musée 2026*) ;
   - une **description** éventuelle ;
   - le(s) **fichier(s)** image(s) à **téléverser**.
3. **Enregistrez** (`gallery.store`). Les photos apparaissent dans la **galerie du site**.

## ✏️ Modifier une galerie
1. Icône **Modifier** (`gallery.edit`) → changez titre/description → `gallery.update`.
2. Pour **ajouter des photos** à un album existant : éditez et re-téléversez.

## 🔴 Supprimer
- **Supprimer une galerie entière** : icône **Supprimer** (`gallery.destroy`), confirmez.
- **Supprimer un seul fichier/image** d'un album, sans toucher au reste :
  `gallery.delete` (`file/delete/{id}`). ⚠️ Retire **définitivement** cette image.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** : galerie **et** fichiers supprimés sont **perdus** ; il faut
  **re-téléverser** les images. **Conservez toujours vos originaux** sur votre ordinateur.

## ⚠️ Bon à savoir
- **Un album = un événement** : titrez clairement pour retrouver facilement les photos.
- **Retrait ciblé** : préférez `gallery.delete` (une image) à la suppression de tout l'album.
- **Droit à l'image** : ne publiez que des photos **autorisées** (élèves, événements publics).
- **Poids des fichiers** : des images trop lourdes **ralentissent** le site — compressez.
- **Différent du diaporama** (*09-diaporama-slider.md*) : le slider est la **bannière
  défilante** de l'accueil ; la galerie est l'**album complet** consultable.
