---
id: 15-06-coordonnees-gps
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-06-coordonnees-gps
emoji: "📍"
titre: "Coordonnées GPS de l'école (géorepérage des présences)"
resume: "Cette page enregistre la position exacte de l'école sur la carte (latitude, longitude) et le rayon autorisé autour de l'établissement."
audiences: [school_admin]
---
# 📍 Coordonnées GPS de l'école (géorepérage des présences)

## 🎯 Rôle
Cette page enregistre la **position exacte de l'école sur la carte** (latitude, longitude) et
le **rayon autorisé** autour de l'établissement. C'est le **gardien géographique** des
présences par **scan QR** : un élève/enseignant ne peut pointer sa présence que **s'il se
trouve dans le périmètre** défini. Sans ce réglage, le contrôle par localisation est
désactivé.

## ✅ Prérequis
1. Être **School Admin** (permission « school-setting-manage »).
2. Connaître les **coordonnées GPS** de l'école (les récupérer gratuitement : ouvrir
   Google Maps sur place → clic droit sur le point → copier **latitude,longitude**).
3. Accès : **Paramètres → GPS Settings** (`school-settings.gps-settings`).

## 🟢 Configurer le GPS (étape par étape)
1. Ouvrez **GPS Settings**.
2. Saisissez la **latitude** (entre -90 et 90) et la **longitude** (entre -180 et 180).
3. Réglez le **rayon de scan QR** en mètres (`qr_scan_radius_meters`, de **10 à 5000**) :
   distance maximum autour de l'école où le scan de présence est accepté.
4. **Enregistrez** (`school-settings.gps-settings.update`).
5. **Testez le jour même** : scannez une présence **depuis l'école** (doit passer) puis
   **dehors** (doit être refusé).

## ✏️ Modifier
1. Revenez sur la page, ajustez coordonnées/rayon, **enregistrez**.
2. Un **rayon trop serré** (ex. 10 m) refuse des élèves pourtant arrivés (imprécision GPS
   des téléphones) : visez **100-300 m** selon la taille du site.

## 🔴 Supprimer / ♻️ Restaurer
- ⚠️ **Effacer les coordonnées = désactiver le géorepérage** : le scan QR redevient possible
  **partout**. Pour rétablir la sécurité, **remettez les coordonnées** (restauration =
  resaisie).
- Il n'y a **pas d'historique** de ce réglage : **notez vos coordonnées** quelque part avant
  toute modification.

## ⚠️ Bon à savoir
- **Le GPS du téléphone pilote** : la précision dépend de l'appareil de l'élève, pas de
  l'école — prévoyez large.
- **Un seul point GPS** : pour un campus à plusieurs bâtiments éloignés, placez le point **au
  centre** et augmentez le rayon.
- **Pas de carte affichée** ici : on saisit des **nombres** ; utilisez Google Maps à côté pour
  vérifier.
- Sans ce réglage, les **présences QR** restent fonctionnelles mais **sans contrôle de
  lieu** — risqué pour les écoles surveillées.
- La **validation EMECEP/intégrations** (test de connexion) est un autre réglage
  (`school-settings.test-emecef`).
