---
id: 12-01-cantine-menus-plats
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-01-cantine-menus-plats
emoji: "🍲"
titre: "Cantine : plats et menus de la semaine"
resume: "La cantine se construit en deux temps : d'abord un catalogue de plats (avec photo et prix enfant / adulte), puis des menus hebdomadaires qui placent ces plats sur les jours de la semaine."
audiences: [school_admin, staff]
---
# 🍲 Cantine : plats et menus de la semaine

## 🎯 Rôle
La **cantine** se construit en deux temps : d'abord un **catalogue de plats** (avec photo et
prix enfant / adulte), puis des **menus hebdomadaires** qui placent ces plats sur les jours
de la semaine. C'est la **carte** que les parents/élèves consultent et qui déclenche les
**réservations** (*02-cantine-reservations-commandes.md*).

## ✅ Prérequis
1. Option « **Canteen Management** » souscrite + permissions cantine.
2. Avoir des **élèves** (la cantine leur est destinée).
3. Accès : menu **Cantine → Dishes** (`canteen.dishes.index`) et **Cantine → Menus**
   (`canteen.menus.index`).

## 🍽️ Créer les plats (catalogue) — étape par étape
1. Ouvrez **Dishes** (plats de la cantine).
2. **Ajouter un plat** (`canteen.dishes.store`) : **nom du plat**, **prix enfant** et
   **prix adulte** (pré-remplis automatiquement selon les tarifs de l'école), catégorie
   éventuelle.
3. **Photo du plat** : uploadez une image via l'action photo (`canteen.dishes.photo`) — une
   belle photo encourage les réservations.
4. **Modifier** un plat : ouvrez sa fiche, corrigez nom/prix, **enregistrez**.
5. Les plats restent dans le **catalogue** et servent à composer les menus.

## 📅 Composer le menu de la semaine — étape par étape
1. Ouvrez **Menus** : la semaine s'affiche en **onglets/jours** (Lundi → Vendredi…).
2. Naviguez **semaine précédente / suivante** (paramètre `week_start`).
3. Sur chaque jour, **ajoutez un plat** du catalogue au menu (`canteen.menus.quick`) —
   création **rapide en ligne**.
4. **Gagner du temps** : bouton **« Dupliquer la semaine précédente »**
   (`canteen.menus.duplicate-previous`) pour reconduire un menu type.
5. **Retirer un plat** d'un jour : supprimez la ligne du menu (le plat reste au catalogue).

## ✏️ Modifier / 🔴 Retirer
- **Modifier un menu** : remplacez un plat par un autre sur le jour voulu (re-ajout via
  `canteen.menus.quick`).
- **Retirer un plat de la carte** : on le **désactive** / ne le reprogramme simplement plus
  la semaine suivante ; le catalogue de plats se gère par **ajouts** (logique « quick add »).

## ♻️ Restaurer
- Les **plats** et **menus** de la cantine fonctionnent par **ajout / re-programmation**,
  pas par corbeille : pour « retrouver » un plat retiré, **re-ajoutez-le** au catalogue ou
  **dupliquez une semaine** qui le contenait.
- Un menu d'une **semaine passée** n'est pas supprimé : il reste consultable pour l'historique.

## ⚠️ Bon à savoir
- **Prix enfant vs adulte** : prévus dès le formulaire — surveillants/enseignants paient le
  tarif adulte.
- **Photos** : misez sur de belles photos de plats, ça **booste les réservations**.
- **Un plat = réutilisable** dans toutes les semaines ; le **menu** ne fait que l'**affecter
  à un jour**.
- La **commande/réservation** et les **statistiques de frequentation** se voient dans *02*.
- L'**encaissement cantine** (espèces / Mobile Money, reçus 58 mm) se fait dans
  **Comptabilité → Cantine** (*PARTIE 10 — 13-comptabilite*).
