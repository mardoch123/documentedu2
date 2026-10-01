---
id: 18-11-cantine
partie: 18
titre_partie: "Application EduStudent"
app: edustudent
slug: 18-11-cantine
emoji: "🍽️"
titre: "la cantine de l'enfant (menu, solde, rechargement USSD)"
resume: "Gérer la restauration scolaire depuis la famille : voir le menu du jour, le solde du compte cantine de l'enfant, l'historique des repas, et recharger le compte par USSD (sans app"
audiences: [parent, student]
---
# 🍽️ 18.11 — EduStudent : la cantine de l'enfant (menu, solde, rechargement USSD)

## 🎯 Rôle
Gérer la **restauration scolaire** depuis la famille : voir le **menu du jour**, le
**solde** du compte cantine de l'enfant, l'**historique des repas**, et recharger le
compte par **USSD** (sans application bancaire).

## ✅ Prérequis
1. Être connecté en parent (page 18.1) et sélectionner l'enfant (page 18.3).
2. Que l'école ait activé la **cantine** avec menus et tarifs (PARTIE 12).
3. Une ligne mobile money active pour le rechargement USSD.

## 🟢 Consulter la cantine
1. Menu enfant → tuile **« Cantine »**.
2. Écran d'accueil cantine : **solde disponible**, **menu de la semaine** (plats,
   tarifs), jour courant mis en évidence.
3. Si le solde couvre le repas du jour, l'enfant est **servi normalement** au
   pointage de l'école (page 17.27) — sinon, prévenir.

## 🟢 Historique des repas
1. Bouton **« Historique »** (canteenHistory) : liste des jours avec repas
   **consommés / non consommés**.
2. Chaque ligne (détails) : date, menu servi, montant débité, solde après repas.
3. Outil idéal pour répondre à « mon enfant a-t-il mangé aujourd'hui ? » sans appeler
  l'école.

## 🟢 Recharger le compte par USSD (étape par étape)
1. Écran cantine → **« Recharger (USSD) »** (canteenUssdTopup).
2. Entrer le **montant** à recharger.
3. L'app affiche le **numéro USSD de l'école** et la marche à suivre (opérateur,
   référence à communiquer) — composez le numéro sur le téléphone.
4. Validez le retrait côté **opérateur** (PIN mobile money).
5. Confirmez dans l'app (référence SMS si demandé) : la transaction apparaît dans
   l'historique USSD, en attente de validation école.
6. Dès la validation de l'école, le **solde cantine augmente** et le rechargement
   passe dans l'historique normal.

## ✏️ / 🔴 / ♻️
- Rien d'éditable côté famille : les **menus et tarifs** vivent sur le web (PARTIE 12).
- Repas consommé à tort (mauvais pointage) : le parent **signale** via le cahier ou un
  message ; l'agent cantine corrige son registre (page 17.27).
- Rechargement USSD débité mais solde inchangé : vérifier d'abord l'**attente de
  validation** école ; si elle traîne, transmettre la référence SMS au secrétariat.
- Solde négatif affiché : normalement le blocage intervient au pointage — un solde
  négatif visible est une anomalie de synchronisation, à signaler.

## ⚠️ Bon à savoir
- Le **solde cantine est séparé** des frais de scolarité : payer la cantine ne paie
  pas les échéances, et inversement.
- Les **jours de fête / suspension de cantine** apparaissent au menu : pas de débit
  sans repas programmé.
- L'historique de repas est la **preuve alimentaire** en cas de réclamation médicale
  (allergène) : conservez-le si votre enfant a un régime suivi (page 18.13).
- Un enfant **changeant de régime** (allergie déclarée en santé) : l'école doit être
  prévenue par le canal santé, pas seulement la cantine.
