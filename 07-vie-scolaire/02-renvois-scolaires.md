---
id: 07-02-renvois-scolaires
partie: 7
titre_partie: "Vie scolaire & discipline"
app: web
slug: 07-02-renvois-scolaires
emoji: "🚫"
titre: "Renvois scolaires pour impayés (liste du jour + règles)"
resume: "Ce module aide la direction à gérer les élèves à renvoyer pour frais non payés, de façon encadrée et manuelle : le logiciel dresse une liste de candidats au renvoi selon les règles que vous définis..."
audiences: [school_admin, staff]
---
# 🚫 Renvois scolaires pour impayés (liste du jour + règles)

## 🎯 Rôle
Ce module aide la direction à **gérer les élèves à renvoyer pour frais non payés**, de façon
**encadrée et manuelle** : le logiciel **dresse une liste de candidats au renvoi** selon les
**règles** que vous définissez (chaque tranche de frais est évaluée selon **son propre dernier
délai**), puis **vous décidez élève par élève** — notification du parent, exécution du renvoi,
ou annulation. **Rien n'est automatique** : aucun élève n'est renvoyé sans votre clic.

## ✅ Prérequis
1. Avoir parametré les **Règles de renvoi** (bouton en haut de page → *Paramètres → Règles de
   renvoi*) : montants, délais, tranches concernées.
2. Avoir saisi les **frais et paiements** des élèves (module Frais).
3. Être **direction / rôle autorisé** (ce module est sensible, souvent masqué aux professeurs).
4. Accès : menu **Vie scolaire → Renvois scolaires** (liste + historique).

## 📊 Lire la synthèse du jour
Quatre cartes (KPI) en haut :
- **À renvoyer aujourd'hui** (`DUE_TODAY`) — la liste du jour à traiter ;
- **À risque (J-2)** (`AT_RISK_J2`) — élèves à **J-2 du délai** : à notifier en priorité ;
- **Renvois exécutés** — historique des renvois déjà validés ;
- **Régularisés / à jour** — élèves qui ont payé entre-temps (à retirer de la liste).

## 🟢 Traiter les renvois du jour (étape par étape)
1. Ouvrez **Vie scolaire → Renvois scolaires**.
2. (Optionnel) Cliquez sur **« Actualiser la liste du jour »** pour recalculer les candidats
   selon les règles et les paiements les plus récents.
3. Filtrez si besoin par **Date de la liste**, **Statut** (Tous / À renvoyer aujourd'hui /
   À risque J-2 / Renvoyé) et **Classe**.
4. Sur chaque ligne, lisez la **« Règle déclenchée et détails »** (motif du candidacy :
   tranche impayée, date limite dépassée…).
5. Choisissez l'action sur la ligne :
   - **Notifier 📣** : envoie l'avis de renvoi au parent (avant toute exécution) ;
   - **Exécuter le renvoi ⚖️** (icône gavel) : **valide manuellement** le renvoi de l'élève —
     disponible uniquement si l'élève est `DUE_TODAY` ou `AT_RISK_J2` et pas déjà renvoyé ;
   - **Annuler ✖** : retire l'élève de la liste (ex. paiement reçu, erreur).

## ✏️ Modifier les règles de renvoi
1. Bouton **« Règles de renvoi »** (⚙️) en haut de la page → *Paramètres de l'école →
   Règles de renvoi*.
2. Ajustez les **critères** (tranches, montants, délais) qui déclenchent une mise en liste.
3. Enregistrez, puis **« Actualiser la liste du jour »** pour recalculer avec les nouvelles
   règles.

## 🔴 Annuler un renvoi exécuté par erreur
- Utilisez **Annuler ✖** sur la ligne tant qu'elle est dans la liste.
- Si l'élève a déjà été **renvoyé** (badge « Renvoyé ») et que c'est une erreur : il faut le
  **ré-intégrer** via **Élèves → Info Apprenant → onglet Inactive → « Active »**
  (voir *06-eleves/03-modifier-supprimer-restaurer-eleve.md*), puis régler sa situation de frais.

## ♻️ Restaurer / réintégrer un élève renvoyé à tort
1. **Élèves → Info Apprenant → onglet « Inactive »**.
2. Retrouvez l'élève renvoyé → cochez → **« Active »** → confirmez.
3. L'élève revient avec tout son historique ; replacez-le dans la bonne classe si besoin.
> Un renvoi **n'efface jamais** la fiche : il désactive l'accès. C'est réversible.

## ⚠️ Bon à savoir
- **Notifiez avant d'exécuter** : la séquence correcte est J-2 (Notifier) → délai → jour J
  (Exécuter). Ne sautez pas la notification.
- Un élève qui **paie entre-temps** bascule en **« Régularisés / à jour »** : vérifiez cette
  carte **avant** d'exécuter un renvoi, pour ne pas punir un parent qui a réglé.
- Le calcul se base sur le **dernier délai de chaque tranche** : un élève peut être « à risque »
  pour une tranche et à jour pour une autre.
- Ce module est **sensible** (impact sur l'enfant) : gardez une **décision humaine** et une
  trace des échanges avec la famille.
