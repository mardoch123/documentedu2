---
id: 11-08-conges-approuver
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-08-conges-approuver
emoji: "✔️"
titre: "Approuver les congés + Gestion des congés (politique annuelle)"
resume: "Cette page couvre deux volets complémentaires : 1."
audiences: [school_admin]
---
# ✔️ Approuver les congés + Gestion des congés (politique annuelle)

## 🎯 Rôle
Cette page couvre **deux volets** complémentaires :
1. **Approuver / rejeter** les demandes de congé déposées par le personnel (*07*) ;
2. **Gestion des congés (leave-master)** : définir la **politique de congés de l'année
   scolaire** — le **nombre de jours de congé** accordés et les **jours de repos
   hebdomadaires** — qui sert de référence à toutes les demandes de l'année.

## ✅ Prérequis
1. Option « **Staff Leave Management** ».
2. Pour **approuver** : permission de gestion des congés (direction / School Admin).
3. Pour **définir la politique** : permission « **school-setting-manage** ».
4. Accès : menu **Leave → Staff Leave** (`leave.request`) pour valider ; menu
   **Paramètres → Gestion des Congés** (`leave-master.index`) pour la politique.

## 🟢 Définir la politique de congés de l'année (étape par étape)
1. Ouvrez **Gestion des Congés** (`leave-master.index`).
2. Cliquez **« Ajouter »** (`leave-master.create`) et renseignez :
   - **Année scolaire (session_year_id)** ★ — **une seule politique par année** (si l'année
     est déjà prise : « Cette année scolaire a déjà été prise. ») ;
   - **Nombre de congés (leaves)** ★ — total de **jours de congé** accordés dans l'année ;
   - **Jours de repos (holiday_days)** ★ — le ou les **jours de la semaine** chômés
     (ex. dimanche, samedi…).
3. **Enregistrez** (`leave-master.store`). Cette politique devient le **cadre** des demandes
   de l'année.
> **Modifier / Supprimer** : `leave-master.edit` / `leave-master.update` /
> `leave-master.destroy`. Une politique supprimée se **recrée** (pas de corbeille).

## ✔️ Approuver ou rejeter une demande
1. Ouvrez **Staff Leave** (`leave.request`) : liste des **demandes en attente**.
2. Cliquez sur une demande pour le **détail** (`leave.request.show`) : période, motif,
   justificatifs joints.
3. Vérifiez la **disponibilité** (autres absences, effectif) puis **changez le statut**
   (`leave.status.update`, PUT) :
   - **Approuvé** : le congé est **validé** (et compté dans la paie si payé) ;
   - **Rejeté** : la demande est **refusée** (l'agent en est informé).

## 📊 Suivi global
- **Rapport de congés** (`leave.report`) : synthèse des congés approuvés/refusés de l'année,
  exportable.
- **Détail** d'une demande (`leave.detail`) et **filtres** (`leave.filter`) par statut/période.

## ♻️ Restaurer
- **Demandes traitées** : pas de restauration ; pour **revenir** sur une décision,
  **changez à nouveau le statut** de la demande (`leave.status.update`).
- **Politique annuelle** supprimée : la **recréer** pour la même année (`leave-master.store`) ;
  ses valeurs (jours, repos) doivent être re-saisies.

## ⚠️ Bon à savoir
- **Une politique par année scolaire** : configurez-la **en début d'année** avant que les
  demandes n'arrivent (sinon les agents ne pourront pas sélectionner l'année).
- **Jours de repos hebdo** : ils influent sur le **calcul des jours ouvrés** des congés et
  sur l'emploi du temps.
- Un congé **approuvé** impacte la **paie** (congés payés autorisés) — voir *PARTIE 10 —
  12-paie*.
- **Traitez les demandes rapidement** : une demande « en attente » bloque la visibilité de
  l'agent sur ses droits restants.
- Le **rejet** doit idéalement s'appuyer sur le **motif** et la **disponibilité** : gardez
  une trace (le rapport d'année sert d'archive).
