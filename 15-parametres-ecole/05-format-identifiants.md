---
id: 15-05-format-identifiants
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-05-format-identifiants
emoji: "🔢"
titre: "Format des identifiants (matricules auto-générés)"
resume: "Cette page définit comment sont fabriqués automatiquement les numéros d'identification (matricules) des élèves, enseignants et membres du personnel : préfixe, nombre de chiffres, suite logique."
audiences: [school_admin]
---
# 🔢 Format des identifiants (matricules auto-générés)

## 🎯 Rôle
Cette page définit **comment sont fabriqués automatiquement les numéros d'identification**
(matricules) des **élèves**, **enseignants** et **membres du personnel** : **préfixe**,
**nombre de chiffres**, suite logique. Un bon format = des matricules **clairs, uniques et
professionnels** (ex. `EDU-2026-0001`), repris sur cartes d'identité, bulletins et apps.

## ✅ Prérequis
1. Être **School Admin**.
2. Avoir **réfléchi au format** avec la direction AVANT la première admission de masse :
   changer de format en cours d'année sème le doute chez les parents.
3. Accès : **Paramètres → ID Formats** (`school-settings.id-formats`).

## 🟢 Configurer le format (étape par étape)
1. Ouvrez **Format des identifiants**.
2. Pour chaque catégorie (élève / enseignant / personnel), réglez :
   - le **préfixe** (ex. *EDU*, *CM*, année en cours) ;
   - le **nombre de chiffres** de la suite (ex. 4 → `0001`, `0002`…) ;
   - les options proposées (inclure l'**année**, reprise de numérotation…).
3. **Enregistrez** (`school-settings.id-formats.store`).
4. Les **créations suivantes** d'élèves/personnel utilisent le nouveau format ; le **format
   global de lettrage** peut aussi être **généré/re-généré** pour les comptes existants
   (voir *Académique → Lettrage/Matricules*).

## ✏️ Modifier le format
1. Revenez sur la page, ajustez préfixe/chiffres, **enregistrez**.
2. ⚠️ Les matricules **déjà attribués ne changent pas** automatiquement : pour uniformiser,
   utilisez l'outil de **régénération des matricules** du module Académique, de préférence
   en **début d'année scolaire**.

## 🔴 Supprimer / ♻️ Restaurer
- Le **format** est un réglage continu : il se **remplace** (Modifier), il ne se supprime ni
  ne se restaure.
- Un **matricule attribué** à un élève se corrige via sa **fiche élève** (ou l'outil de
  lettrage) — pas ici.

## ⚠️ Bon à savoir
- **Restez court** : un matricule de 6-10 caractères se dicte et se retient ; 25 caractères,
  non.
- **Un préfixe par école** évite les collisions si vous changez de plateforme un jour.
- **Ne réutilisez jamais** un matricule d'élève sorti pour un nouvel élève : l'historique
  (paiements, bulletins) est rattaché à ce numéro.
- Le matricule sert aussi d'**identifiant de connexion** dans les apps mobiles : communiquez
  le format aux parents à l'admission.
- Les **numéros de reçus** ont leur propre réglage (*03, code de reçu*).
