---
id: 11-07-conges-demander
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-07-conges-demander
emoji: "✈️"
titre: "Demander un congé (prof / personnel) + rapport"
resume: "Chaque enseignant et membre du personnel peut demander un congé depuis son espace : il choisit le type de congé, la période, expose le motif et joint éventuellement un justificatif."
audiences: [school_admin, teacher, staff]
---
# ✈️ Demander un congé (prof / personnel) + rapport

## 🎯 Rôle
Chaque **enseignant** et **membre du personnel** peut **demander un congé** depuis son
espace : il choisit le **type de congé**, la **période**, expose le **motif** et joint
éventuellement un **justificatif**. La demande part ensuite en **validation** (voir
*08-conges-approuver.md*). Le **rapport de congés** permet à chacun (et à la direction) de
**consulter l'historique** des congés posés et acceptés.

## ✅ Prérequis
1. Option « **Staff Leave Management** » + permission « **leave-create** ».
2. Avoir une **politique de congés** configurée pour l'**année scolaire** (voir *08*,
   Gestion des congés / `leave-master`).
3. Accès : menu **Leave → Apply Leave** (`leave.index`).

## 🟢 Demander un congé (étape par étape)
1. Ouvrez **Apply Leave** puis le **formulaire de demande** (`leave.request.show`).
2. Renseignez :
   - **Droit de congé de l'année (leave_master_id)** ★ — la **politique de congés** de
     l'**année scolaire** en cours (nombre de jours autorisés + jours de repos hebdo),
     définie par l'école en *08-conges-approuver.md* ;
   - **Du (from_date)** ★ et **Au (to_date)** ★ — la période (la fin doit être **≥ au
     début**) ;
   - **Type de journée** (`type`) — ex. **journée entière / demi-journée** ;
   - **Motif (reason)** ★ — explication de la demande ;
   - **Justificatifs (files)** — facultatif : formats **jpg, jpeg, png, pdf, doc, docx**,
     dans la **limite de taille** fixée par l'école.
3. **Envoyer la demande** (`leave.store`). Statut initial : **en attente** de validation.

## 📋 Consulter mes congés
- **Ma liste** : `leave.index` montre mes demandes avec leur **statut**
  (en attente / approuvé / rejeté).
- **Détail d'une demande** : `leave.detail`.
- **Filtrer** : `leave.filter` (par période, statut, type).

## 📊 Rapport de congés (Leave Report)
- Menu **Leave → Leave Report** (`leave.report`) : **synthèse** des congés (qui, quand,
  combien de jours), exportable. Utile à la direction pour **anticiper les absences**.

## ✏️ Annuler / modifier ma demande
- Une demande **encore « en attente »** peut être **reprise** (modifier / retirer) par son
  auteur tant qu'elle n'est pas traitée (`leave.edit` / `leave.destroy`).
- Une fois **approuvée**, la modification passe par la **direction** (voir *08*).

## 🔴 Supprimer / ♻️ Restaurer
- Supprimer ma propre demande (`leave.destroy`) l'**efface** du circuit.
- ⚠️ Pas de **corbeille** pour les demandes de congé : une demande annulée se **recrée** en
  reposant une nouvelle demande. Consultez le **rapport** pour retrouver la trace d'un congé
  déjà validé.

## ⚠️ Bon à savoir
- **Les congés validés influent sur la paie** : les **jours de congé payés autorisés**
  entrent dans le calcul du salaire (voir *PARTIE 10 — 12-paie* et *09-fiches-de-paie-slip*).
- **Respectez la limite de taille des fichiers** : un justificatif trop lourd est refusé.
- **to_date ≥ from_date** : impossible de terminer un congé avant son début.
- Le **type de congé** (payé / non payé / nombre de jours autorisés) est défini par
  l'école dans la **Gestion des congés** (*08*) : demandez le **bon type**.
- Conservez une **copie de vos justificatifs** (maladie…) : la demande supprimée n'est pas
  récupérable.
