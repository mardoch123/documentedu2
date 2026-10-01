---
id: 17-21-config-moyens-paiement-ussd
partie: 17
titre_partie: "Application EduStaff"
app: edustaff
slug: 17-21-config-moyens-paiement-ussd
emoji: "🔧"
titre: "EduStaff (direction) : configurer les moyens de paiement et l'USSD"
resume: "Depuis le téléphone, activer et tester tout ce qui fait entrer l'argent à l'école : caisse espèces, FeexPay (mobile money/cartes), KKiaPay, et les comptes USSD par pays/opérateur"
audiences: [teacher, staff, school_admin]
---
# 🔧 17.21 — EduStaff (direction) : configurer les moyens de paiement et l'USSD

## 🎯 Rôle
Depuis le téléphone, **activer et tester** tout ce qui fait entrer l'argent à l'école :
**caisse espèces**, **FeexPay** (mobile money/cartes), **KKiaPay**, et les **comptes
USSD** par pays/opérateur — plus l'imprimante des reçus.

## ✅ Prérequis
1. Être **School Admin** (ou délégation « payment_config », page 17.25).
2. Avoir ses **clés API** fournies par FeexPay/KKiaPay (comptes marchand de l'école).
3. Comprendre que ces réglages touchent **l'argent de toute l'école** : on ne les
   modifie pas « pour voir ».

## 🟢 Ouvrir le hub « Moyens de paiement »
1. Accueil → **« + »** → famille **Outils** → **« Config. moyens de paiement »**
   (ou badge ⚙️ de l'écran d'accueil direction).
2. Le hub présente **4 cartes** : **Caisse / Espèces**, **FeexPay**, **KKiaPay**,
   **USSD**. Chaque carte s'ouvre en formulaire ; les clés affichées sont
   **masquées** (début…fin) — jamais en clair.

## 🟢 Activer une passerelle (FeexPay ou KKiaPay)
1. Ouvrir la carte (ex. **FeexPay**) : saisir **public key / secret key / shop id**
   selon les champs du formulaire (erreurs affichées en français).
2. Cocher **Sandbox (test)** pendant les essais, décocher pour la production.
3. Bouton **« Tester la connexion »** — ⚠️ à faire **avant** d'enregistrer : le test
   dit si les clés sont bonnes.
4. Bouton **« Enregistrer »** : la sauvegarde relance un test automatique.
5. Le **historique des modifications** (auteur + date, 50 dernières) reste consultable
   en bas de l'écran.

## 🟢 Configurer les comptes USSD
1. Carte **USSD** du hub (ou tuile « Config. USSD »).
2. Choisir le **pays** : **Bénin, Guinée, Côte d'Ivoire, Sénégal, Togo,
   Burkina Faso**.
3. Pour chaque **opérateur** du pays, activer le compte (MTN MoMo, Moov Money,
   Orange, Wave… selon pays) — **maximum 5 comptes** activés.
4. Chaque compte affiche son **numéro USSD généré** (celui que les parents composent)
   et un bouton **« Tester »** pour vérifier la réception.
5. Option **code personnalisé** par école : si l'opérateur local exige un format
   différent, le modèle peut être adapté (sinon le modèle catalogue s'applique).

## 🟢 Suivre et valider les paiements USSD reçus
1. Famille **Encaissement & Paiements** → **« Paiements USSD (admin) »**.
2. **Liste** des transactions déclarées par les parents (montant, opérateur,
   référence) ; ouvrez une ligne pour le **détail complet**.
3. **Valider** impute le paiement sur le frais de l'élève — voyez page 17.20.

## 🟢 Imprimante thermique
1. Famille **Outils** → **« Imprimante thermique »** : choisir l'imprimante **58 mm**
   appairée en Bluetooth, tester l'impression d'un bandeau.

## ✏️ Modifier / 🔴 désactiver
- Tout se **rémodifie** dans le même hub : tester puis enregistrer à chaque fois.
- **Désactiver** une passerelle = l'enregistrer en mode inactif (ou sans clés) : les
  parents ne voient plus ce canal de paiement, l'historique reste.
- ⚠️ Ne supprimez jamais un compte USSD **encore publié** sur les affiches de l'école :
  changez d'abord les supports.

## ♻️ Restaurer
- Clés perdues/changées chez FeexPay : ressaisir les nouvelles, **Tester**, Enregistrer.
- Écran refuse d'ouvrir (« Accès refusé ») : votre compte n'a plus la délégation —
  page 17.25 ou web.
- Paiement USSD effectué mais absent de la liste : le parent doit donner la
  **référence exacte du SMS opérateur** ; vérifiez aussi les filtres de dates, puis
  validez la transaction réparée dès que la passerelle refonctionne.

## ⚠️ Bon à savoir
- **Toujours tester avant d'enregistrer** en production ; une passerelle mal configurée =
  parents facturés sans que l'école voie arriver l'argent.
- Les **clés complètes ne s'affichent jamais** dans l'app (masquées) : c'est une
  sécurité, pas un bug.
- Les **5 comptes USSD maximum** protègent contre la confusion parentale : gardez les
  opérateurs réellement utilisés par vos familles.
- Le web garde la **priorité** pour les cas complexes (PARTIE 10) ; l'app est faite
  pour les ajustements rapides et les contrôles terrain.
