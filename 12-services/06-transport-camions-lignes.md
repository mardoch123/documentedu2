---
id: 12-06-transport-camions-lignes
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-06-transport-camions-lignes
emoji: "🔗"
titre: "Transport : associer véhicules ↔ lignes"
resume: "Cette page marie un véhicule (03) à une ligne (05) : « le Bus 01 roule sur la ligne Centre-Ville »."
audiences: [school_admin, staff]
---
# 🔗 Transport : associer véhicules ↔ lignes

## 🎯 Rôle
Cette page **marie un véhicule** (*03*) **à une ligne** (*05*) : « le Bus 01 roule sur la
ligne Centre-Ville ». Une **association véhicule-ligne** porte les informations
d'exploitation (quel bus, quelle ligne, éventuellement créneau). Cycle complet géré :
**créer, modifier, supprimer (corbeille), restaurer**.

## ✅ Prérequis
1. Avoir créé au moins un **véhicule** (*03*) et une **ligne** (*05*).
2. Option « **Transport Management** » + permissions route-vehicle.
3. Accès : menu **Transport → Route Vehicle** (`route-vehicle.index`).

## 🟢 Créer une association véhicule ↔ ligne (étape par étape)
1. Ouvrez **Route Vehicle**, cliquez **« Ajouter »** (`route-vehicle.create`).
2. Sélectionnez :
   - le **Véhicule** (parmi le parc, *03*) ;
   - la **Ligne** (parmi les lignes, *05*) ;
   - tout paramètre d'exploitation proposé (chauffeur/aide via *07*, horaires éventuels).
3. **Enregistrez** (`route-vehicle.store`). L'association apparaît : le véhicule **roule
   désormais sur cette ligne**.

## ✏️ Modifier une association
1. Icône **Modifier** (`route-vehicle.edit`) → changez véhicule/ligne/paramètres →
   `route-vehicle.update`.
   > Utile pour **remplacer un bus tombé en panne** par un autre sur la même ligne.

## 🔴 Supprimer une association (corbeille)
1. Icône **Supprimer** (`route-vehicle.destroy`), confirmez.
2. L'association part à la **corbeille** : le véhicule **n'est plus lié** à la ligne, mais
   l'entrée reste **récupérable**.
3. Basculez **« all | Trashed »** sur **« Trashed »** pour la voir.
4. Depuis « Trashed », la **suppression définitive** (`route-vehicle.trash`) efface pour bon.

## ♻️ Restaurer une association supprimée
1. Liste en mode **« Trashed »**.
2. Cliquez **Restaurer** (`route-vehicle.restore`, `route-vehicle/{id}/restore`).
3. L'association **revient** : le véhicule est **de nouveau affecté** à sa ligne.

## ⚠️ Bon à savoir
- **Un véhicule peut desservir plusieurs lignes** (à des créneaux différents) et **une ligne
  peut avoir plusieurs véhicules** : l'association est la « baguette » qui les relie.
- **Remplacer un véhicule** = modifier l'association (*✏️*) plutôt que tout recréer : les
  élèves affectés à la ligne ne sont pas perturbés.
- ⚠️ **Supprimer une association** peut **laisser une ligne sans bus** : vérifiez qu'une
  autre coverte la ligne avant de supprimer.
- **Restauration disponible** : en cas de suppression douteuse, l'onglet « Trashed » +
  Restaurer remet tout en place.
- Les **conducteurs** (chauffeurs/aides) se gèrent dans *07-transport-chauffeurs-aides.md* et
  se rattachent ici ou sur la ligne selon l'école.
