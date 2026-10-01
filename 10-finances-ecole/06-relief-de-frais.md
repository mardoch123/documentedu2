---
id: 10-06-relief-de-frais
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-06-relief-de-frais
emoji: "🤝"
titre: "Manage Fee Relief (secours / remises accordées)"
resume: "Manage Fee Relief est l'outil de secours financier de l'école : on accorde une aide ponctuelle (remise globale) à un élève, en montant fixe ou en pourcentage, avec une date et une description du mo..."
audiences: [school_admin, staff]
---
# 🤝 Manage Fee Relief (secours / remises accordées)

## 🎯 Rôle
**Manage Fee Relief** est l'outil de **secours financier** de l'école : on accorde une
**aide ponctuelle** (remise globale) à un élève, en **montant fixe** ou en **pourcentage**,
avec une **date** et une **description** du motif. Contrairement à la réduction ciblée
(*05*), le secours est **saisi en un bloc** et surtout il dispose d'un **journal
d'actions** et d'un bouton **Rollback** pour **annuler** proprement un secours accordé par
erreur. C'est la fonction à privilégier quand on veut pouvoir **revenir en arrière**.

## ✅ Prérequis
1. Option « **Fees Management** » + permission « **fees-paid** ».
2. Élève déjà **facturé** (grille de frais *02*).
3. Accès : menu **Fees → Manage Fee Relief** (`fees.discount.index`).

## 🟢 Accorder un secours (étape par étape)
1. Ouvrez **Manage Fee Relief**.
2. Sélectionnez la **Classe** puis l'**Élève** (recherche élève `fees.discount.students-by-class`,
   détail de ses frais `fees.discount.student-fees` / `fees.discount.fee-details`).
3. Renseignez le formulaire de secours :
   - **« discount_name »** ★ — nom du secours (ex. « Bourse solidarité ») ;
   - **Type de remise** ★ : **Fixe** (montant FCFA) ou **Pourcentage** (`fixed` / `percentage`) ;
   - **Valeur** ★ (`discount_value`, minimum 1) — le champ affiche par ex. « E.g., 1000 » ;
   - **Date du secours** ★ (`discount_date`) ;
   - **Description / motif** — texte libre expliquant la raison.
4. **Enregistrez** (`fees.discount.store`). Le secours vient **diminuer le reste à payer**
   de l'élève.

## 📋 Consulter les secours et le journal
- **Liste des secours accordés** : bouton de la liste (`fees.discount.list`) — colonnes élève,
  nom du secours, type, valeur, date.
- **Journal d'actions** (`fees.discount.logs`) : historique **traçable** de chaque
  attribution et de chaque **rollback** (qui, quand, anciennes données conservées).

## 🔴 Annuler un secours (Rollback)
1. Sur la ligne du secours, cliquez le **bouton d'annulation / Rollback**.
2. L'action `fees.discount.rollback/{id}` **supprime le secours** et **restaure le montant
   initial** de la facture.
3. Une **entrée « rollback »** est ajoutée au **journal** (avec les anciennes données) :
   l'annulation est **totalement traçable**.

## ♻️ Restaurer / rétablir
- Le **Rollback** est le mécanisme d'annulation propre : après un rollback, pour **rétablir**
  le secours, il suffit de l'**accorder à nouveau** (même formulaire). Grâce au **journal**,
  vous retrouvez exactement le **nom, type, valeur et date** du secours annulé.
- Il n'y a **pas d'onglet « Trashed »** : le suivi se fait via le **journal des actions**,
  plus fiable qu'une corbeille.

## ⚠️ Bon à savoir
- **Rollback = annulation sûre** : à la différence de *05* (suppression définitive), ici
  chaque suppression est **journalisée** avec l'**ancienne valeur** conservée → on peut
  recréer à l'identique sans rien perdre de l'information.
- **Fixe vs Pourcentage** : le fixe retire un **montant FCFA** précis ; le pourcentage retire
  un **%** du frais (attention aux gros frais, l'effet est plus grand).
- Ne **cumulez pas** un secours (*06*) et une réduction ciblée (*05*) sur le **même frais**
  sans vérifier le reste à payer final : les deux systèmes se **retrouvent additionnés**
  dans la facture de l'élève.
- Le **journal** (`fees.discount.logs`) est votre **preuve** en cas de litige : expliquez-y
  toujours le motif.
