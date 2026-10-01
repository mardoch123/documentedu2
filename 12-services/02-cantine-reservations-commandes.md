---
id: 12-02-cantine-reservations-commandes
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-02-cantine-reservations-commandes
emoji: "🍛"
titre: "Cantine : réservations, service du jour et statistiques"
resume: "Cette page gère le quotidien de la cantine : qui a réservé quel repas et quel jour, comment servir les élèves au moment du déjeuner, comment réserver en masse, et les statistiques de fréquentation."
audiences: [school_admin, staff]
---
# 🍛 Cantine : réservations, service du jour et statistiques

## 🎯 Rôle
Cette page gère le **quotidien de la cantine** : qui a **réservé** quel repas et quel jour,
comment **servir** les élèves au moment du déjeuner, comment **réserver en masse**, et les
**statistiques** de fréquentation. Elle s'appuie sur les **menus/plats** définis dans *01*.

## ✅ Prérequis
1. Avoir **publié les menus de la semaine** (*01-cantine-menus-plats.md*).
2. Option « **Canteen Management** » + permissions réservations.
3. Accès : menu **Cantine → Reservations** (`canteen.reservations.index`) et
  **Cantine → Dashboard** (`canteen.dashboard`).

## 🟢 Réserver des repas (étape par étape)
1. Ouvrez **Reservations** : la grille des **élèves × jours** de la semaine s'affiche.
2. Filtrez par **classe** ; **recherchez un élève** (`canteen.reservations.search-students`).
3. Trois façons de réserver :
   - **Un élève / un jour** : basculez sa case (`canteen.reservations.toggle-student`) ;
   - **Réserve rapide** pour un élève (`canteen.reservations.quick`) ;
   - **Réserver pour toute la classe** d'un coup (`canteen.reservations.reserve-all`).
4. La réservation est **enregistrée** : l'élève (ou le parent depuis son app) la voit.

## 🍽️ Servir au déjeuner (pointage du jour)
1. Le jour dit, ouvrez la liste des **réservants**.
2. Au passage de l'élève, marquez-le **servi** (`canteen.reservations.serve-student`) : le
   compteur de portions consommées se met à jour.
3. Cela permet de **compter les couverts** réels et de **facturer** ce qui a été mangé.

## 📊 Tableau de bord & statistiques
- **Dashboard cantine** (`canteen.dashboard`) : **vue du jour** (réservés, servis, restants).
- **Statistiques** (`canteen.statistics`) : **fréquentation** par jour / classe / période —
  utile pour ajuster les quantités cuisinées.
- **Liste cuisine** (`canteen.reservations.export-kitchen`) : **PDF des quantités** à
  préparer, envoyé en **cuisine**.

## ✏️ Annuler / modifier une réservation
- **Annuler** : rebasculez la case de l'élève (`toggle-student`) → la réservation saute.
- **Modifier le menu réservé** : l'élève change de jour ou de plat via les mêmes actions
  rapides.

## 🔴 Supprimer / ♻️ Restaurer
- Les réservations ne vont **pas à la corbeille** : on les **annule** (case décochée) ou on
  ne les **ressert pas**. Une réservation annulée se **re-crée** en 1 clic (`quick` /
  `toggle-student`).
- L'**historique** (statistiques) reste consultable : rien n'est « perdu », c'est juste un
  **état**.

## ⚠️ Bon à savoir
- **Réserver tôt = cuisiner juste** : les **statistiques** évitent le gaspillage (trop ou
  pas assez de portions).
- Les **parents** peuvent réserver/effectuer un solde depuis leur **app mobile** (EduStudent)
  ou l'**espace parent**, selon la configuration — les chiffres tombent ici.
- Le **règlement** (solde cantine, rechargement, espèces/Mobile Money) se traite dans
  **Comptabilité → Cantine** (*13*) ; cette page gère **qui mange quoi, quand**.
- **Export cuisine PDF** : préparez la **liste des quantités** la veille.
- Pensez à **servir (pointer)** chaque midi pour des **statistiques fiables**.
