---
id: 11-03-supprimer-restaurer-enseignant
partie: 11
titre_partie: "Enseignants & personnel"
app: web
slug: 11-03-supprimer-restaurer-enseignant
emoji: "🗑️"
titre: "Supprimer, désactiver et restaurer un enseignant"
resume: "Un enseignant peut partir définitivement (départ, fin de contrat) ou être mis en pause congé sabbatique, inactivité."
audiences: [school_admin]
---
# 🗑️ Supprimer, désactiver et restaurer un enseignant

## 🎯 Rôle
Un enseignant peut partir **définitivement** (départ, fin de contrat) ou être mis **en pause**
congé sabbatique, inactivité. Ce module couvre les **trois gestes** : **désactiver**
(suspendre l'accès sans effacer), **supprimer** (mettre à la **corbeille**) et **restaurer**
(remettre un enseignant supprimé en activité). Choisir le bon geste évite de **perdre**
inutilement un historique (notes, affectations, paie).

## ✅ Prérequis
1. Permission « **teacher-delete** » (suppression) / « teacher-edit » (statut).
2. Accès : menu **Teacher → Manage Teacher** (`teachers.index`), ligne de l'enseignant.

## ⏸️ Désactiver un enseignant (recommandé)
La **désactivation** conserve la fiche et **coupe l'accès** : c'est le geste **sûr**.
1. Sur la ligne de l'enseignant, utilisez le **changement de statut** (`teachers.change-status`) :
   passez le **Statut** de **actif → inactif** (case ou bouton de la ligne).
2. L'enseignant **n'est plus actif** (plus de connexion, plus d'affectations proposées) mais
   **reste dans la base** avec tout son historique.
3. Pour **réactiver**, refaites `teachers.change-status` → **actif**.
> **Changement en masse** : cochez plusieurs lignes puis **`change-status-bulk`** pour
> activer/désactiver d'un coup.

## 🔴 Supprimer un enseignant (corbeille)
1. Sur la ligne, cliquez l'**icône Supprimer**, puis **confirmez**.
2. L'enseignant part à la **corbeille** (`teachers.trash`) : il **disparaît** de la liste
   active mais **reste récupérable**.
3. Basculez le sélecteur **« all | Trashed »** (au-dessus du tableau) sur **« Trashed »** pour
   **voir les enseignants supprimés**.
4. Depuis « Trashed », une **suppression définitive** efface pour de bon (irréversible).

## ♻️ Restaurer un enseignant supprimé
1. Passez la liste en mode **« Trashed »**.
2. Cliquez l'**icône Restaurer** sur l'enseignant voulu (`teachers.restore`).
3. L'enseignant **revient dans la liste active**, avec ses **matières, affectations et
   historique** conservés.

## ⚠️ Bon à savoir
- **Préférez désactiver à supprimer** : un enseignant **supprimé définitivement** perd ses
  liens (notes, paie) ; un enseignant **inactif** garde tout et se réactive en 1 clic.
- **Corbeille = filet de sécurité** : après une suppression, vous avez toujours l'onglet
  **« Trashed »** + **Restaurer** pour revenir en arrière.
- **Email libéré ?** Un email d'enseignant supprimé **définitivement** peut parfois être
  réutilisé ; tant qu'il est en **corbeille**, l'email reste **pris** (donc un nouveau
  compte avec le même email sera refusé).
- Supprimer un enseignant **ne supprime pas** les **bulletins/notes** déjà saisis (ils
  restent rattachés à la classe) — voir PARTIE Examens.
- Ces trois gestes (statut / corbeille / restauration) existent **à l'identique pour le
  personnel non enseignant** (*04-administration-personnel-staff.md*).
