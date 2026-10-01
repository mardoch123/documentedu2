---
id: 17-27-services-annexes
partie: 17
titre_partie: "Application EduStaff"
app: edustaff
slug: 17-27-services-annexes
emoji: "🍲"
titre: "cantine, bibliothèque, mobilier et santé depuis l'app"
resume: "Les gestes terrain des services annexes, sans ordinateur : pointer les repas distribués, suivre le stock de la cantine, scanner un livre ou un meuble, consigner une fiche médical"
audiences: [teacher, staff, school_admin]
---
# 🍲 17.27 — EduStaff : cantine, bibliothèque, mobilier et santé depuis l'app

## 🎯 Rôle
Les **gestes terrain** des services annexes, sans ordinateur : pointer les repas
distribués, suivre le **stock de la cantine**, **scanner** un livre ou un meuble,
consigner une **fiche médicale** — les paramètres complements restent sur le web
(PARTIE 12).

## ✅ Prérequis
1. Être School Admin ou agent de service habilité (cantinier, bibliothécaire,
   infirmier).
2. Que le module concerné soit **activé pour l'école** (web, PARTIE 12/15).

## 🟢 Cantine : stock et distribution
1. Écran **« Cantine »** (famille Outils ou tuile dédiée).
2. **Stock** : la liste des denrées avec quantités ; **ajouter / réduire** une ligne
   à chaque livraison ou retrait d'utilisation — l'écran suit les mêmes champs que le web.
3. **Distribution** : cocher les **bénéficiaires du jour** (élèves/agents) ou scanner la
   liste ; le repas du jour est sélectionné en en-tête.
4. En fin de journée, **valider la distribution** : les consommations déduisent le
   stock et alimentent le coût de revient web.

## 🟢 Bibliothèque : scanner et inventorier
1. Écran **« Bibliothèque »** → quatre zones : **Accueil, Scanner, Inventaire,
   Stats**.
2. **Scanner** : cadrer le **code-barres/QR du livre** → l'exemplaire s'ouvre :
   **emprunter** pour un élève (nom + classe), ou **retourner**.
3. **Inventaire** : recherche, ajout d'exemplaires (même formulaire que le web),
   correction d'état (abîmé, perdu).
4. **Stats** : emprunts du jour/mois, livres les plus sortis — lecture rapide.

## 🟢 Mobilier : inventaire et maintenance
1. Écran **« Mobilier »** : Accueil / **Scanner** / Inventaire / **Maintenance**.
2. **Scanner la carte d'un meuble** (table, banc, armoire) : sa fiche s'ouvre —
   état, salle, historique.
3. **Signaler une maintenance** depuis la fiche : nature de la panne, photo,
   urgence → la ligne passe dans la liste « Maintenance » de la direction.
4. **Inventaire** : compter par salle, corriger les déplacements.

## 🟢 Santé : l'espace infirmier
1. Écran **« Santé (personnel soignant) »**.
2. Rechercher l'**élève**, ouvrir son **dossier** (allergies, groupes sanguins,
   visites antérieures selon ce que l'école a saisi).
3. **Consigner une consultation** : motif, geste effectué, recommandation — les
   parents la verront sur EduStudent (rubrique santé).

## ✏️ Modifier
- Chaque ligne (stock, exemplaire, meuble, dossier) s'édite depuis sa fiche :
  changer quantité, état, salle → **Enregistrer**.

## 🔴 Supprimer
- **Stock** : on **ajuste la quantité**, on ne supprime pas une ligne historisée.
- Un **exemplaire de bibliothèque** retiré (réformé) : changement d'**état**, pas
  suppression — l'historique des emprunts doit survivre.
- Une consultation santé se **corrige tant qu'elle n'est pas validée** ; après,
  ajouter une note rectificative.

## ♻️ Restaurer
- Fiche introuvable au scanner : le QR/codes-barres n'est pas celui de l'école —
  vérifier l'étiquette, ou retrouver la fiche par **recherche manuelle** dans
  l'inventaire.
- Distribution de cantine effacée : redistribuer la liste du jour (les élèves
  concernés gardent leur compteur web intact).
- Meuble sans étiquette lisible : la direction **réimprime** une carte depuis le web
  (PARTIE 12 mobilier).

## ⚠️ Bon à savoir
- Ces écrans sont des **saisies rapides** : les gros paramétrages (menus de cantine,
  rayons, catégories de mobilier) se font sur le web PARTIE 12.
- Le scanner fonctionne **hors ligne partiellement** (file d'attente) mais la
  synchronisation exige Internet : finir chaque journée connecté.
- Un stock cantine faux se voit vite : le **coût du jour** affiché en stats diverge —
  re-compter avant la clôture hebdo.
- Santé : ne consigner que des **faits médicaux objectifs** — les données santé sont
  sensibles et consultables par la seule infirmerie/parents.
