---
id: 06-08-promotion-en-masse
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-08-promotion-en-masse
emoji: "🎓"
titre: "Promotion en masse des élèves (fin d'année)"
resume: "À la fin de l'année, faire monter toute une classe vers la classe supérieure d'un seul geste, en tenant compte des moyennes : le logiciel calcule la moyenne générale de chaque élève, sépare les adm..."
audiences: [school_admin, staff]
---
# 🎓 Promotion en masse des élèves (fin d'année)

## 🎯 Rôle
À la fin de l'année, faire **monter toute une classe vers la classe supérieure** d'un seul
geste, en tenant compte des **moyennes** : le logiciel calcule la moyenne générale de chaque
élève, sépare les **admises** des **non admises**, et envoie les admis en classe
supérieure pendant que les non-admis **redoublent** automatiquement. C'est l'outil de clôture
de cycle le plus important de l'année.

## ✅ Prérequis
1. Avoir **saisi toutes les notes / bulletins** de l'année (sinon les moyennes sont fausses).
2. Avoir **créé la classe de destination** (la classe supérieure) dans *Structure → Classes*,
   sinon les élèves resteront bloqués dans leur classe actuelle.
3. Avoir défini la **nouvelle année / période** de destination.
4. Permission « student-edit ».
5. Accès : menu **Élèves → Promotion en masse** (badge AVANCÉ).

## 🟢 Déroulé complet (étape par étape)
### 1. Configurer la promotion
1. Choisissez la **Classe de départ** ★ (liste groupée par classe, affichant
   « Filière – Section (Classe) »).
2. Réglez la **Moyenne minimale pour passer** (par défaut **10 /20**, modifiable de 0 à 20
   par pas de 0,5).
3. Cliquez sur **« Calculer les moyennes »**.
> La moyenne générale est calculée **automatiquement sur tous les trimestres disponibles** :
> somme des moyennes de trimestres ÷ nombre de trimestres, **pondérée par les coefficients**
> des matières. Vous n'avez rien à calculer vous-même.

### 2. Lire les résultats
Quatre cartes statistiques apparaissent :
- **Élèves dans la classe** (total),
- **Admis (moyenne atteinte)** — verts,
- **Non admis** — rouges,
- **Moyenne de la classe /20** + anneau du **taux de réussite %**.

### 3. Choisir la destination et les options
1. Dans **« Classe d'arrivée (destination) »**, sélectionnez la classe supérieure.
   ⚠️ Si un bandeau d'alerte dit « Cette classe est la dernière niveau », créez d'abord la
   classe de destination dans le menu **Classes**, sinon les élèves resteront en place.
2. Option **« Redoublant automatique des non-admis »** (case) : les élèves **sans la moyenne**
   sont repositionnés **dans la même classe** avec la nouvelle période (ils redoublent
   proprement au lieu de rester bloqués administrativement). **Fortement recommandé de la
   cocher.**
3. Cochez les élèves à promouvoir (case par case, ou **« Tout sélectionner »**).

### 4. Lancer
Cliquez sur **« Promouvoir les élèves sélectionnés »** → confirmez.
Un historique **« Dernières opérations sur cet appareil »** garde la trace des promotions
lancées (utile pour vérifier ce qui a été fait).

## ✏️ Annuler / corriger une promotion mal lancée
- La promotion **déplace** les élèves vers la classe/section de destination : pour « revenir
  en arrière », relancez une **rétrogradation** en choisissant l'ancienne classe comme
  **destination** (même outil, classe de départ = la nouvelle classe).
- Pour un **seul** élève mal placé : **Info Apprenant → Modifier** → étape Affectation →
  remettez la bonne classe → Mettre à jour.
- Pour un redoublant devenu admis (moyenne corrigée après coup) : passez-le individuellement
  en classe supérieure via sa fiche.

## 🔴 Supprimer une promotion de toute une classe
Il n'y a pas de bouton « supprimer la promotion » : on la **corrige en re-promouvant dans
l'autre sens** (voir ✏️ ci-dessus). C'est pour cela qu'il faut **vérifier les moyennes AVANT**
de cliquer sur « Promouvoir ».

## ♻️ Retrouver des élèves « disparus » après promotion
Ils ne sont pas supprimés, ils ont **changé de classe** : regardez dans la **classe de
destination** (ou la même classe si redoublants). Vérifiez aussi l'onglet **« Inactive »** de
**Info Apprenant** au cas où un seuil de moyenne les aurait fait basculer.

## ⚠️ Bon à savoir
- **Faites un test** sur une petite classe avant de promouvoir tout l'établissement.
- Cochez **« Redoublant automatique des non-admis »** : sinon les non-admis restent
  administrativement bloqués dans l'ancienne période.
- La promotion **ne génère pas** les bulletins de la nouvelle année : c'est une étape
  séparée des examens.
- Après promotion, pensez à **attribuer les matricules** de la nouvelle classe
  (*05-academique-mobilite/03-numeros-matricules.md*).
