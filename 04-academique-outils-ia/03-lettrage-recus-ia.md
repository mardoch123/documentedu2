---
id: 04-03-lettrage-recus-ia
partie: 4
titre_partie: "Académique : Outils IA"
app: web
slug: 04-03-lettrage-recus-ia
emoji: "📘"
titre: "Lettrage & Reçus IA (relances impayés)"
resume: "Transformer la longue liste des impayés en actions prêtes à envoyer : l'outil « Lettrage » apparie automatiquement les paiements déclarés avec les factures dues (qui a payé quoi,"
audiences: [school_admin]
---
# Lettrage & Reçus IA (relances impayés)

## 🎯 Rôle
Transformer la longue liste des **impayés** en actions prêtes à envoyer : l'outil
« Lettrage » **apparie automatiquement** les paiements déclarés avec les factures dues
(qui a payé quoi, reste-t-il un solde ?) et génère des **courriers/reçus de relance
personnalisés par parent** (WhatsApp, email ou PDF à imprimer), rédigés par l'IA.

## ✅ Prérequis
- Des **frais** attribués aux classes et des **paiements** enregistrés
  (voir [10-finances-ecole/03-paiements-eleves.md](../10-finances-ecole/03-paiements-eleves.md)).
- Accès : menu **Académique → Lettrage & Reçus IA**.

## 🟢 Étape 1 — Lancer le lettrage (rapprochement)
1. Ouvrez **Lettrage & Reçus IA**.
2. Choisissez la **période / le semestre** et la classe à contrôler.
3. Cliquez sur **Lancer le rapprochement**.
4. Le tableau affiche trois colonnes :
   - ✅ **Payés** : tout correspond, rien à faire ;
   - ⚠️ **Partiels** : un solde reste dû (montant affiché) ;
   - ❓ **À vérifier** : paiement sans facture correspondante (ou l'inverse) —
     examinez chaque ligne et corrigez l'imputation via le crayon ✏️.

## 🟢 Étape 2 — Générer les reçus / lettres de relance
1. Filtrez sur les lignes **Partiels** (les clients à relancer).
2. Sélectionnez les parents concernés (cases à cocher) ou « tout sélectionner ».
3. Cliquez sur **Générer les reçus/relances IA**.
4. Choisissez le **canal** : PDF imprimable, email, ou message WhatsApp (selon vos modules
   activés) et le **ton** du message (courtois / ferme / dernière relance).
5. Une **prévisualisation** s'affiche : relisez ! L'IA insère les vrais montants mais peut
   rester à peaufiner (le texte signalé « [à compléter] » doit être corrigé).
6. Validez l'**envoi** (ou le téléchargement du lot PDF). Chaque envoi est tracé dans
   le *Journal & Logs SMS/WhatsApp*.

## ✏️ Corriger un rapprochement
- Paiement mal imputé → icône **crayon ✏️** sur la ligne « À vérifier » →
  réaffectez-le au bon frais de l'élève → enregistrer.
- Paiement non saisi → retournez dans *Élèves → Paiements* pour l'enregistrer d'abord,
  puis relancez le lettrage.

## 🔴 Supprimer / annuler une relance
Une relance **envoyée** ne se rattrape pas (le message est parti). Vous pouvez seulement :
1. Ignorer la ligne dans l'outil (bouton **Ignorer / Masquer**) pour ne plus la relancer ;
2. Ou annuler l'**envoi planifié** s'il est encore en file (bouton ✕ sur la tâche en attente).

## ♻️ Restaurer
Les étiquettes « ignorées » se réactivent en changeant le filtre de statut
(« Ignorés » → ligne → **Réinclure**). Les rapprochements se recalculent à chaque
nouvelle lancette : rien n'est définitif.

## ⚠️ Bon à savoir
- Vérifiez le **numéro WhatsApp du parent** avant d'envoyer par ce canal
  (fiche parent → téléphone validé, +228/… au bon format).
- Ne laissez jamais un solde « négatif » (trop-perçu) sans explication : l'outil le
  signale en rouge — remboursez ou compensez sur le prochain frais.
- Les lettres générées mentionnent des **montants réels** : le contrôle de lecture par
  un humain avant envoi est une obligation, pas une option.
