---
id: 10-12-paie
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-12-paie
emoji: "💵"
titre: "Paie du personnel (payroll + paramètres)"
resume: "Le module Paie (Payroll) prépare et génère la paie mensuelle du personnel (enseignants et staff) : salaire de base, congés payés autorisés, indemnités, retenues, puis fiche de paie (slip) imprimable."
audiences: [school_admin, staff]
---
# 💵 Paie du personnel (payroll + paramètres)

## 🎯 Rôle
Le module **Paie (Payroll)** prépare et **génère la paie mensuelle** du personnel
(enseignants et staff) : salaire de base, **congés payés autorisés**, indemnités, retenues,
puis **fiche de paie (slip)** imprimable. Les **paramètres de paie (Payroll Setting)**
définissent à l'avance la **structure de salaire** de chaque membre (base, allowances,
deductions) pour alimenter la génération.

## ✅ Prérequis
1. Avoir des **enseignants / staff** avec une **structure de paie** renseignée.
2. Permissions « **payroll** » (génération) et « payroll-setting » (paramètres).
3. Accès : menu **Finances → Paie** (`payroll.index`) et **Paramètres de paie**
   (`payroll-setting.index`).

## ⚙️ Préparer les paramètres de paie (cycle complet)
Avant de générer, on définit la **structure** de chaque membre.
1. **Créer** : **Paramètres de paie** → « Ajouter » → choisir le **membre**, saisir le
   **salaire de base**, les **indemnités (allowances)** et **retenues (deductions)**, les
   **congés payés mensuels autorisés**, puis **Enregistrer** (`payroll-setting.store`).
2. **Modifier** : icône **Modifier** → ajuster → `payroll-setting.update`.
3. **Supprimer (corbeille)** : icône **Supprimer** → la structure part à la **corbeille**
   (`payroll-setting.trash`). Basculez **« all | Trashed »** sur **« Trashed »**.
4. **Restaurer** : depuis « Trashed », **Restaurer** (`payroll-setting.restore`) → la
   structure revient. ✅ **Les paramètres de paie sont restaurables.**

## 🟢 Générer la paie d'un mois (étape par étape)
1. Ouvrez **Paie** (`payroll.index`).
2. Sélectionnez le **Mois** ★ et l'**Année** ★ (champ **month** + **year**), utilisez la
   **recherche** pour filtrer le personnel.
3. Cliquez **« Créer la paie »** / **« Generate »** (`payroll.store`) : la liste du personnel
   avec son **salaire de base** (`basic_salary`) et ses **congés payés autorisés**
   (*Monthly Allowed Paid Leaves*) se prépare pour la **date** ★ du mois.
4. Ajustez éventuellement le **montant à payer** (input **salary**) ligne par ligne
   (heures sup., absences, primes).
5. **Validez la génération** : les entrées de paie du mois sont créées, chacune avec son
   **statut**.

## 🧾 Consulter / imprimer une fiche de paie (slip)
- **Liste des fiches** : `payroll.slip.index` (toutes les fiches).
- **Fiche d'un membre** : `payroll.slip/{id}` — détail **base + indemnités − retenues = net
  à payer**, **imprimable / téléchargeable** (PDF). Le membre peut aussi voir **ses propres
  fiches** depuis son espace (voir *PARTIE 11 — fiches de paie*).

## 🔴 Supprimer une paie générée
1. Sur l'entrée de paie, icône **Supprimer** (`payroll.destroy`), confirmez.
2. ⚠️ L'entrée de paie est **définitivement effacée** (la paie n'a **pas de corbeille**, pas
   de modification non plus : on **supprime puis on régénère**).

## ♻️ Restaurer
- **Entrées de paie** : ⚠️ **pas de restauration** — pour corriger une paie supprimée ou
  erronée, **régénérez le mois** (le module ne propose ni édition ni corbeille : la
  méthode officielle est **supprimer → régénérer**).
- **Paramètres de paie** : ✅ restaurables via « Trashed » + Restaurer (voir ⚙️).

## ⚠️ Bon à savoir
- **Pas de bouton « Modifier » sur la paie** : le flux est **stock / show / destroy** ; pour
  un ajustement, on **supprime l'entrée du mois** et on la **régénère** avec les bonnes
  valeurs.
- La **structure de paie** (base, allowances, deductions) se corrige dans les **Paramètres
  de paie** (*restaurables*), pas dans la paie du mois.
- **Congés payés autorisés** : les jours de congé déjà validés (module Congés, *PARTIE 11*)
  impactent le calcul — vérifiez les congés avant de générer.
- La paie **ne passe pas** par le module Dépenses : c'est un **circuit séparé**.
- Conservez les **fiches (slips)** PDF : ce sont les **justificatifs** remis au personnel.
