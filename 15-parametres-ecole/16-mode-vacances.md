---
id: 15-16-mode-vacances
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-16-mode-vacances
emoji: "🏖️"
titre: "Mode vacances de l'école"
resume: "Un interrupteur « école fermée » : quand vous l'activez pendant les grandes vacances (ou une période creuse), l'application adapte son comportement — les écrans/notifications signalent que l'établi..."
audiences: [school_admin]
---
# 🏖️ Mode vacances de l'école

## 🎯 Rôle
Un interrupteur **« école fermée »** : quand vous l'activez pendant les grandes vacances (ou
une période creuse), l'application **adapte son comportement** — les écrans/notifications
signalent que l'établissement est en congé, les cycles quotidiens (présences, cours) passent
en **pause visible** pour les familles et le personnel, puis tout **reprend** à la rentrée
sans ressaisie. C'est le « panneau FERMÉ » numérique de l'école.

## ✅ Prérequis
1. Être **School Admin**.
2. Avoir déclaré les **jours fériés/vacances** correspondants (*PARTIE 13, 08*) pour la
   cohérence du calendrier.
3. Accès : **Paramètres → Vacation Mode** (`vacation-mode.index`).

## 🟢 Activer le mode vacances (étape par étape)
1. Ouvrez **Mode Vacances**.
2. Consultez l'état du jour (`vacation-mode.status`) : « Activé / Désactivé ».
3. Basculez l'interrupteur **ON** → **Enregistrer** (`vacation-mode.toggle`).
4. **Vérifiez** : le site/espace famille affiche le congé ; les envois quotidiens non
   essentiels se calment.

## 🟢 Désactiver à la rentrée
1. Même page → interrupteur **OFF** → **Enregistrer** (`vacation-mode.toggle`).
2. Reprenez les gestes normaux : **année/session active**, emplois du temps, présences.

## ✏️ Modifier / 🔴 Supprimer / ♻️ Restaurer
- Simple **interrupteur** : pas de création, pas de suppression, rien à restaurer — on
  **bascule** dans un sens ou dans l'autre, à tout moment, sans effet destructeur.
- ⚠️ Ne l'oubliez **pas activé** en septembre : une école « en vacances » qui ne notifie plus
  les parents crée des malentendus — mettez-vous un **rappel calendrier** pour la rentrée.

## ⚠️ Bon à savoir
- **Différence avec les jours fériés** (*PARTIE 13-08*) : les fériés datent des **périodes
  précises** dans le calendrier ; le mode vacances est un **état global** de l'école.
- **Pendant les vacances**, profitez-en pour les gros travaux : nouvelle **session
  scolaire** (*02*), **points de restauration** (*13*), **prospectus de rentrée**
  (*PARTIE 14-07*).
- Le mode vacances ne **bloque pas** votre accès admin : vous pouvez continuer à travailler.
- En cas de **doute sur l'état visible** par les parents, testez avec un compte parent ou
  l'app mobile.
