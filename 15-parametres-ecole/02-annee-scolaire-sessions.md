---
id: 15-02-annee-scolaire-sessions
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-02-annee-scolaire-sessions
emoji: "🗓️"
titre: "Année / session scolaire (créer, activer, clôturer)"
resume: "La session scolaire (année scolaire, ex."
audiences: [school_admin]
---
# 🗓️ Année / session scolaire (créer, activer, clôturer)

## 🎯 Rôle
La **session scolaire** (année scolaire, ex. *2026-2027*) est le **cadre temporel master** de
toute l'activité : notes, présences, frais, examens et rapports y sont rattachés. On y
associe des **semestres/trimestres** (périodes d'évaluation et de facturation). Savoir
**créer la nouvelle année**, la **rendre active** et **archiver l'ancienne** est le geste le
plus important de la rentrée.

## ✅ Prérequis
1. Être **School Admin**.
2. Avoir défini les **dates de rentrée/clôture** de l'année.
3. Accès : menu **Academics → Session Year** (`session-year.index`) ; les semestres se gèrent
   dans **Semester** (PARTIE Académique).

## 🟢 Créer une année scolaire (étape par étape)
1. Ouvrez **Session Year** → **« Ajouter »**.
2. Saisissez le **nom de l'année** (ex. *2026-2027*) et les **dates** début/fin.
3. **Enregistrez** (`session-year.store`).
4. **Créez ses semestres/trimestres** dans le module **Semester** (1, 2 ou 3 selon votre
   organisation), rattachés à cette année.

## 🚀 Activer l'année (le geste crucial)
1. Dans la liste des années, repérez la nouvelle année.
2. Cliquez sur **« Set Default / Par défaut »** (`session-year.default`) — un **anneau/icone
   actif** signale l'année **en cours d'utilisation**.
3. Toute la saisie (notes, frais, présences) se fait désormais dans cette année.
   > Astuce : l'option **`session-year.set-session-year`** permet aussi de choisir l'année
   > courante depuis les filtres globaux.

## ✏️ Modifier une année
1. Icône **Modifier** (`session-year.edit`) → corrigez nom/dates → `session-year.update`.
   ⚠️ Ne changez les **dates** qu'avec soin : bulletins et rapports s'en servent.

## 🔴 Supprimer une année (corbeille)
1. Icône **Supprimer** (`session-year.trash`, `session-year/{id}/deleted`).
2. L'année part en **corbeille** ; basculez **« all | Trashed »** sur **« Trashed »**.
3. Depuis « Trashed », suppression **définitive** possible.
   > ⚠️ **Ne supprimez jamais une année contenant des résultats définitifs** : archivez en la
   > laissant simplement **non active**.

## ♻️ Restaurer une année
1. Passez le filtre sur **« Trashed »**.
2. Cliquez **Restaurer** (`session-year.restore`) → l'année revient avec ses **semestres et
   données**.

## 🧹 Nettoyer les données d'une année
- **Avant archivage** : consultez le rapport de nettoyage (`session-year.cleanup-info/{id}`)
  puis lancez le **nettoyage ciblé** (`session-year.cleanup-data/{id}`) pour retirer les
  données de **test** (attention : opération **réflexion faite**, données de test uniquement).

## ⚠️ Bon à savoir
- **Une seule année active** : les anciennes restent consultables (historique) en changeant
  le filtre d'année.
- **Ordre des opérations à la rentrée** : créer l'année → créer ses semestres → **activer** →
  promouvoir les élèves → rouvrir les frais.
- Le **choix du semestre actif** se fait via **Set Semester** (`set-semester`).
- La **politique de congés** annuelle (*module Personnel*) se rattache aussi à l'année.
