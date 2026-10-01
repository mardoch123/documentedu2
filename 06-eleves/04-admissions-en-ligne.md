---
id: 06-04-admissions-en-ligne
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-04-admissions-en-ligne
emoji: "🌐"
titre: "Traiter les demandes d'admission en ligne"
resume: "Quand votre école publie un formulaire d'admission sur son site web (ou un lien/QR code partagé), les familles remplissent la demande elles-mêmes."
audiences: [school_admin, staff]
---
# 🌐 Traiter les demandes d'admission en ligne

## 🎯 Rôle
Quand votre école publie un **formulaire d'admission sur son site web** (ou un lien/QR code
partagé), les familles remplissent la demande **elles-mêmes**. Ce module est la **boîte de
réception** : vous y voyez toutes les demandes arrivées, vous les **acceptez ou rejetez**,
et les demandes acceptées deviennent de vraies fiches élèves.

## ✅ Prérequis
1. Avoir **activé le formulaire d'admission en ligne** pour votre école
   (module *Site web / Formulaire d'intégration* — voir partie Paramètres). L'accès à ce
   module est lié à l'option d'abonnement **« Website Management »**.
2. Permission « student-create ».
3. Avoir créé les **classes** (pour diriger les demandes acceptées).
4. Accès : menu **Élèves → Demandes d'admission** (icône ✉️).

## 📋 Lire la liste des demandes
La liste affiche, pour chaque demande reçue :
- le **Nom** et la **photo** du candidat, sa **date de naissance**, son **sexe**,
- la **classe demandée**, la **date de la demande**,
- le **statut de la demande** (`application_status`) : en attente / **accepted** / **rejected**,
- les coordonnées du **parent** (email, nom, mobile) — colonnes masquées activables via
  le menu **Colonnes 🧭**,
- les **champs du formulaire d'admission** que la famille a remplis (également masqués par
  défaut, à afficher via Colonnes).
Utilisez la **recherche** et les filtres **Classe / Classe-Section** en haut pour trier.

## 🟢 Accepter une demande (étape par étape)
1. Filtrez sur la **Classe** et la **Classe-Section** concernées (cases ★ en haut).
2. Repérez la demande dans la liste ; cliquez sur sa ligne pour voir le détail si besoin.
3. Dans la colonne **Action**, choisissez le statut **Acceptée (accepted)** puis **Soumettre**
   (ou utilisez le crayon ✏️ pour compléter la fiche avant d'accepter).
4. ⚠️ **TRÈS IMPORTANT** : après acceptation, l'élève est créé **en statut INACTIF par défaut**.
   Pour finaliser l'inscription, vous **devez l'activer manuellement** :
   - allez dans **Élèves → Info Apprenant**,
   - ouvrez l'onglet **« Inactive »**, retrouvez l'élève,
   - cochez-le → bouton **« Active »** (voir *03-modifier-supprimer-restaurer-eleve.md*).
   > Sans cette activation, l'élève n'apparaît pas dans les classes actives et ne peut pas
   > être utilisé (présences, frais, appli mobile).

## 🔴 Rejeter une demande
1. Sur la ligne de la demande, colonne **Action**, choisissez **Rejetée (rejected)** → **Soumettre**.
2. La demande passe en statut rejetée (visible via le filtre de statut). Vous pouvez la
   remettre en attente plus tard si la famille se représente.

## ✏️ Compléter / corriger une demande avant décision
1. Crayon **✏️** sur la ligne : le formulaire d'édition de l'élève s'ouvre.
2. Corrigez ou complétez les infos (le parent a pu mal saisir), puis **Mettre à jour**.
3. Revenez accepter la demande (étapes ci-dessus).

## 🔁 Modifier une décision (acceptée / rejetée par erreur)
- Reprenez l'action sur la ligne et changez le statut (**accepted ↔ rejected**) → **Soumettre**.
- Si l'élève accepté doit « repartir » : désactivez-le dans **Info Apprenant** (onglet actif →
  bouton **Inactive**), plutôt que de supprimer.

## ⚠️ Bon à savoir
- **Accepter ≠ inscrire complètement** : pensez toujours à l'**activation manuelle** (étape 4).
  C'est l'erreur n°1 des nouvelles écoles.
- Les demandes en trop / farfelues peuvent rester en attente sans gêner votre fonctionnement.
- La liste est **exportable** (Excel, PDF, CSV…) via l'icône **Export 📤** — pratique pour un
  point hebdomadaire des inscriptions.
- Ce module concerne les **candidatures entrantes du site web** ; les élèves déjà admis se
  gèrent dans **Info Apprenant**.
