---
id: 15-03-moyens-de-paiement-ecole
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-03-moyens-de-paiement-ecole
emoji: "💰"
titre: "Moyens de paiement & devise de l'école"
resume: "Cette page dit au système comment les parents peuvent vous payer : quels moyens de paiement mobile/en ligne sont activés (Mobile Money MTN/Moov, FeexPay, espèces…"
audiences: [school_admin]
---
# 💰 Moyens de paiement & devise de l'école

## 🎯 Rôle
Cette page dit au système **comment les parents peuvent vous payer** : quels **moyens de
paiement mobile/en ligne** sont activés (Mobile Money MTN/Moov, FeexPay, espèces…), dans
quelle **devise** sont libellés les montants (FCFA, GNF, USD…) et quels **comptes** reçoivent
les paiements. Les boutons « Payer » des apps mobiles et des liens de paiement respectent ce
choix.

## ✅ Prérequis
1. Être **School Admin** (menu protégé des enseignants).
2. Avoir un **compte marchand/numéro marchand** actif auprès de l'opérateur choisi (ex.
   numéro MTN MoMo marchand) — sinon activez seulement **Espèces**.
3. Accès : **Paramètres → Payment** (`school-settings.payment.index`) et
   **Currency** (`school-settings.currency`).

## 🟢 Activer des moyens de paiement (étape par étape)
1. Ouvrez **Paramètres → Moyens de paiement**.
2. Cochez/activez les méthodes voulues et renseignez les **identifiants marchands** demandés
   (numéro marchand, clef API FeexPay de l'école, etc.).
3. Définissez les **devises acceptées** si proposé.
4. **Enregistrez** (`school-settings.payment.update`).
5. **Testez** : émettez un lien de paiement vers votre propre numéro et vérifiez la
   **réception** du paiement dans les journaux (*Frais → journal des transactions*).

## 💱 Changer la devise
1. Ouvrez **Paramètres → Currency** (`school-settings.currency`).
2. Choisissez la **devise** (symbole et position) de l'école.
3. **Enregistrez** (`school-settings.currency.store`).
   ⚠️ La devise s'applique aux **nouveaux montants** ; les montants déjà saisis ne sont pas
   convertis — **changez de devise en début d'année**, pas en cours de route.

## ✏️ Modifier
- Revenez sur la page, **activez/désactivez** une méthode, corrigez un **numéro marchand**,
  puis **enregistrez** à nouveau. Une méthode **désactivée** disparaît des boutons de
  paiement sans effacer les **historiques** de paiement.

## 🔴 Supprimer / ♻️ Restaurer
- Ici, rien ne se **supprime** : on **active/désactive**. Un paiement déjà encaissé se
  **corrige** par un **remboursement ou une note** dans le module Frais, pas ici.

## ⚠️ Bon à savoir
- **Espèces toujours possibles** : même sans mobile money, la caisse enregistre les paiements
  (*caisse/PDF reçu*).
- **FeexPay** : si votre école utilise les paiements en ligne EduEasy, les **clefs**
  s'affichent ici ; ne les partagez **qu'avec le Support EduEasy** en cas de problème.
- **Numéro marchand erroné = paiements bloqués** : vérifiez caractère par caractère.
- Les **codes de reçu** (format des numéros de reçu) se règlent dans la même zone Paramètres
  (`school-settings.generate-receipt-code`).
- Le **format des cartes/identifiants** et les pages légales sont traités dans d'autres pages
  de ce dossier.
