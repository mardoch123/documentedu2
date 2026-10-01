---
id: 15-09-notifications-sms-solde
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-09-notifications-sms-solde
emoji: "📲"
titre: "Hub notifications SMS/WhatsApp & solde de crédits"
resume: "C'est le poste de contrôle des communications payantes de l'école : le solde de crédits SMS/WhatsApp, les réglages d'envoi automatiques, l'achat de crédits (rechargement) et un économiseur intellig..."
audiences: [school_admin]
---
# 📲 Hub notifications SMS/WhatsApp & solde de crédits

## 🎯 Rôle
C'est le **poste de contrôle des communications payantes** de l'école : le **solde** de
crédits SMS/WhatsApp, les **réglages** d'envoi automatiques, l'**achat de crédits**
(rechargement) et un **économiseur intelligent** qui choisit le canal le moins cher
(WhatsApp gratuit quand le parent l'a, sinon SMS). Chaque message aux parents **puise dans ce
portefeuille**.

## ✅ Prérequis
1. Être **School Admin**.
2. Accès : **Paramètres → Notifications Hub** (`school-settings.notifications-hub`).
3. Un moyen de paiement actif pour **recharger** (FeexPay/Mobile Money).

## 🟢 Consulter et recharger le solde (étape par étape)
1. Ouvrez **Notifications Hub** : le **solde actuel** de crédits s'affiche en tête.
2. Pour **acheter des crédits** : lancez un **rechargement**
   (`school-settings.notifications-hub.topup`, ou la page dédiée `sms.recharge` →
   `sms.process-recharge` → confirmation `sms.confirm-recharge`).
3. **Payez** via le lien mobile money envoyé ; le solde monte après confirmation
   (`sms.balance` en consultation rapide).
4. ⚠️ Un solde **à zéro bloque les envois SMS** : rechargez **avant** les campagnes
   (rappels de frais, avis d'absence).

## ⚙️ Régler les envois
1. Dans le hub, ajustez les **options d'envoi automatique** (quels événements notifient les
   parents, par quel canal) → `school-settings.notifications-hub.settings`.
2. **Économiseur intelligent** : activez/désactivez le bouton
   `toggle-smart-credit-saver` — avec, le système **préfère WhatsApp** (coût nul) quand le
   parent est joignable ainsi, et **ne prend le SMS** qu'en repli.

## ✏️ Modifier / 🔴 Supprimer / ♻️ Restaurer
- Le hub est un **tableau de réglages continus** : rien à créer/supprimer/restaurer —
  chaque interrupteur s'**inverse** à volonté, **enregistrez** après changement.
- Les **crédits achetés** ne sont pas remboursables : vérifiez le **volume prévu** avant
  gros achat.

## ⚠️ Bon à savoir
- **1 crédit ≈ 1 SMS** : les longues notifications peuvent compter **double** (seuils
  opérateur).
- **WhatsApp = gratuit mais fragile** : le parent doit avoir l'app **et** un numéro
  enregistré ; le SMS passe **partout** mais **coûte**.
- **Suivez la consommation** dans le **journal** (*10*) : une chute bizarre = campagne
 mal déclenchée.
- Les **annonces manuelles** (avec choix SMS/WhatsApp) se font dans le module Annonces ;
  le hub, lui, gouverne les **automatismes et le budget**.
- Le **numéro expéditeur** et les templates WhatsApp se gèrent en *11*.
