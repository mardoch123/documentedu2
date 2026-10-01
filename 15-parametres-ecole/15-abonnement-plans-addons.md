---
id: 15-15-abonnement-plans-addons
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-15-abonnement-plans-addons
emoji: "🎫"
titre: "Mon abonnement : historique, plans & options (addons)"
resume: "C'est votre compteur EduEasy : le forfait (package) choisi par l'école (nb d'élèves, modules inclus, durée), son état (actif, expiré, en essai), son historique, le renouvellement et l'ajout d'optio..."
audiences: [school_admin]
---
# 🎫 Mon abonnement : historique, plans & options (addons)

## 🎯 Rôle
C'est **votre compteur EduEasy** : le **forfait (package)** choisi par l'école (nb d'élèves,
modules inclus, durée), son **état** (actif, expiré, en essai), son **historique**, le
**renouvellement** et l'ajout d'**options payantes (addons)** — cantine, santé, WhatsApp,
modules avancés… Tout ce qui touche **le prix et les droits d'usage** de votre licence se
passe ici.

## ✅ Prérequis
1. Être **School Admin** (la page d'abonnement école est `subscriptions.index` ; les
   forfaits eux-mêmes sont créés **côté plateforme**, pas par vous).
2. Un moyen de paiement opérationnel (*03*).

## 🟢 Souscrire / renouveler un plan (étape par étape)
1. Ouvrez **Mon abonnement / Souscription** (`subscriptions.index`) : les **plans disponibles**
   s'affichent avec **prix et contenu**, plus votre plan actuel.
2. Choisissez le **forfait voulu** → page du plan (`subscriptions/plan/{id}/type/{type}`) →
   éventuellement version **prépayée** (`subscriptions.prepaid.package`).
3. **Sélectionnez le paiement** (`subscriptions.select-payment`) :
   - **FeexPay/Mobile Money** : `subscriptions.feexpay.payment` → callback/success automatique ;
   - **Western Union** : instructions + justificatif (`subscriptions.wu.payment` →
     `wu.submit`) — Validation par EduEasy ensuite ;
   - **Virement bancaire** : idem (`subscriptions.bt.payment` → `bt.submit`).
4. Le plan devient **actif dès confirmation du paiement** ; le **reçu** est téléchargeable
   (`subscriptions.bill/receipt/{id}`).

## 🕘 Consulter l'historique & la suite
- **Historique des abonnements** : `subscriptions.history` (anciens plans, dates, factures).
- **Plan programmé** (upcoming) : un renouvellement déjà payé à date future peut être
  **confirmé** (`subscriptions/confirm-upcoming-plan/{id}`) ou **annulé**
  (`subscriptions.cancel.upcoming`) — l'annulation **remet le plan actuel** sans facturer la
  suite.
- **Ajustement du quota de comptes staff** : `subscriptions.staff-quota.preview` puis
  `staff-quota.adjust` (payer plus de licences personnel).

## ➕ Souscrire une option (addon)
1. Depuis l'espace abonnement, ouvrez les **options/addons** proposées.
2. Choisissez la durée → paiement (FeexPay dédié `addons.feexpay.payment/{id}`).
3. L'option s'**ajoute aux modules actifs** dès paiement.

## ✏️ Modifier / 🔴 Supprimer / ♻️ Restaurer
- On ne « supprime » pas un abonnement payé : on le **laisse expirer** (non-renouvellement)
  ou on **annule le renouvellement programmé** (*cancel-upcoming*).
- ⚠️ **Abonnement expiré** : l'écran « expiré » s'affiche **une seule fois**, ensuite la
  **consultation reste ouverte** mais **les écritures sont bloquées** (plus de saisie de
  notes/paiements) — **renouvelez vite** pour débloquer.
- Un **essai gratuit 14 jours** est proposé aux nouvelles écoles (éligibilité affichée sur la
  page).

## ⚠️ Bon à savoir
- **Le quota élèves/personnel** du plan limite les créations de comptes : avant la rentrée,
  vérifiez la **marge**.
- **Factures** : téléchargez chaque reçu et rangez-les (comptabilité de l'école).
- Le lien « Souscrire » d'un compte expiré mène **toujours** à cette page — pas de piège.
- **Groupes scolaires** : plusieurs écoles sous un même compte ont une formule spéciale
  (*19-groupe-scolaire.md*).
- Pour toute **réclamation** (double débit, plan non reconnu) : contactez le Support avec
  **n° de facture + capture**.
