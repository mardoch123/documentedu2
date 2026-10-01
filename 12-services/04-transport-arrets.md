---
id: 12-04-transport-arrets
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-04-transport-arrets
emoji: "📍"
titre: "Transport : points de ramassage (arrêts)"
resume: "Un point de ramassage (arrêt) est un lieu d'embarquement/débarquement des élèves : « carrefour X », « place Y »…"
audiences: [school_admin, staff]
---
# 📍 Transport : points de ramassage (arrêts)

## 🎯 Rôle
Un **point de ramassage** (arrêt) est un **lieu d'embarquement/débarquement** des élèves :
« carrefour X », « place Y »… Les arrêts sont **regroupés en lignes de transport** (*05*) et
chaque élève est affecté à **un arrêt** de sa ligne. Cette page tient le **répertoire des
arrêts** de l'école.

## ✅ Prérequis
1. Option « **Transport Management** » + permissions pickup point.
2. Accès : menu **Transport → Pickup Points** (`pickup-points.index`).

## 🟢 Créer un point de ramassage (étape par étape)
1. Ouvrez **Pickup Points**, cliquez **« Ajouter »** (`pickup-points.create`).
2. Renseignez :
   - **Nom de l'arrêt** (ex. « Carrefour Kpota ») ;
   - **Localisation / précision** (quartier, repère) ;
   - éventuellement un **ordre** de passage et une **distance/tarification** associée.
3. **Enregistrez** (`pickup-points.store`). L'arrêt est prêt à être **placé sur une ligne**.

## ✏️ Modifier un arrêt
1. Icône **Modifier** (`pickup-points.edit`) → corrigez nom / position →
   `pickup-points.update`.

## 🔗 Placer un arrêt sur une ligne
- Les arrêts s'**organisent en ligne** dans **Routes** (*05*) : c'est là qu'on **ajoute des
  arrêts à une ligne** et qu'on **change leur ordre de passage**
  (`routes.change-order` → `routes.update-pickup-order`).
- Retirer un arrêt d'une ligne : `pickup-points.delete` (sur la route) enlève l'arrêt de la
  **ligne** concernée.

## 🔴 Supprimer un arrêt
1. Icône **Supprimer** (`pickup-points.destroy`), confirmez.
2. ⚠️ L'arrêt est **retiré définitivement** du répertoire.

## ♻️ Restaurer
- ⚠️ Les **points de ramassage ne sont pas restaurables** (pas de corbeille) : un arrêt
  supprimé doit être **recréé**, puis **remis sur ses lignes** (*05*). Notez les arrêts
  importants avant suppression.

## ⚠️ Bon à savoir
- **Nommez les arrêts par des repères clairs** (les parents doivent les reconnaître
  facilement).
- Un arrêt **utilisé par des élèves affectés** ne doit pas être supprimé sans **replacer ces
  élèves** sur un autre arrêt.
- **Un même arrêt** peut servir à **plusieurs lignes** (intersection).
- L'**ordre de passage** des arrêts se gère sur la **ligne** (*05*), pas ici.
- Enchaînement complet du transport : **Arrêts (04) → Lignes (05) → Véhicules (03)
  ↔ Lignes (06) → Chauffeurs (07) → Demande d'affectation élève (05) → Dépenses
  (08)**.
