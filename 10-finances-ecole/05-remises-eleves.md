---
id: 10-05-remises-eleves
partie: 10
titre_partie: "Frais & finances de l'école"
app: web
slug: 10-05-remises-eleves
emoji: "🎓"
titre: "Réductions / bourses sur les frais (Student Fees Discount)"
resume: "Cette fonction (Student Fees Discount) permet d'accorder une remise (bourse, réduction commerciale, geste commercial) sur un frais précis d'un élève : un pourcentage ou un montant fixe retiré du mo..."
audiences: [school_admin, staff]
---
# 🎓 Réductions / bourses sur les frais (Student Fees Discount)

## 🎯 Rôle
Cette fonction (**Student Fees Discount**) permet d'**accorder une remise** (bourse,
réduction commerciale, geste commercial) **sur un frais précis d'un élève** : un
**pourcentage** ou un **montant fixe** retiré du montant à payer. La remise est
**rattachée à un élève + un frais (+ une tranche)**, appliquée par un membre habilité et
**traçable** (qui l'a accordée). À ne **pas confondre** avec *Manage Fee Relief* (*06*) qui,
elle, est un **secours ponctuel global**.

## ✅ Prérequis
1. Option « **Fees Management** » activée + permission « **fees-create** » (accorder) /
   « fees-delete » (retirer).
2. Avoir créé une **grille de frais** (*02*) et des **élèves** déjà facturés.
3. Accès : menu **Fees → Student Fees Discount** (`fees-discount.index`).

## 🟢 Accorder une réduction (étape par étape)
1. Ouvrez **Student Fees Discount** (page « Réductions »).
2. Filtrez par **Année scolaire** puis **Classe/Section** pour retrouver l'élève.
3. Cliquez **« Ajouter une réduction »** (`fees-discount.create`) — ou utilisez
   **« Appliquer en lot »** pour toute une classe (`fees-discount.batch-store`).
4. Renseignez :
   - **Élève** ★ (via la classe/section) ;
   - **Frais concerné** ★ (la facture de l'élève, `fees-discount.get-student-fees`) ;
   - **Tranche** ciblée (ou « **Tous les frais** ») — liste `fees-discount.get-fees-installments` ;
   - **Type de réduction** ★ : **pourcentage** (%) ou **montant fixe** (FCFA) ;
   - **Valeur** ★ de la remise ;
   - **Motif / raison** (`reason`) : ex. « Bourse d'excellence ».
5. **Enregistrez**. Le **montant à payer** de l'élève diminue immédiatement du montant de la
   remise (`discount_amount`).

## 📋 Consulter les réductions accordées
- La liste montre : **Élève, Frais, Tranche, Type, Valeur, Montant remis, Accordée par**.
- Tableau **recherchable / exportable** (Recherche, Colonnes, Rafraîchir, Export).
- On peut **éditer** une remise (`fees-discount.edit` → `fees-discount.update`).

## 🔴 Retirer / annuler une réduction
1. Sur la ligne de la remise, cliquez **Supprimer** puis confirmez.
2. Message « **Réduction supprimée avec succès** » : la remise est **effacée**, le montant
   d'origine **revient** sur la facture de l'élève.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** pour les réductions : une remise supprimée est **définitivement
  effacée**. Pour « retrouver » une remise retirée par erreur, il faut la **recréer**
  (même élève, même frais, même valeur). Notez donc les motifs importants.

## ⚠️ Bon à savoir
- **Deux systèmes de remise coexistent** dans l'application :
  - **Student Fees Discount** (cette page, `fees-discount.*`) : remise **ciblée** sur un frais,
    côté **web/parent** ;
  - **Manage Fee Relief** (*06*, `fees.discount.*`) : **secours global** accordé, avec
    **journal** et **rollback**. Les deux sont **fusionnés en lecture** dans le montant à
    payer de l'élève : ne doublez pas les avantages.
- Une remise **ne peut pas dépasser** le montant du frais.
- **Règle dégressive des tranches** : plus l'élève paie tôt (tranche basse), meilleure est
  la remise automatique prévue par l'école ; renseignez-vous avant d'ajouter une remise
  manuelle.
- Conservez un **motif clair** (`reason`) : c'est votre seule trace en cas de litige, car il
  n'y a pas de restauration.
