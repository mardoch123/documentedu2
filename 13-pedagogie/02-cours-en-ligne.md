---
id: 13-02-cours-en-ligne
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-02-cours-en-ligne
emoji: "💻"
titre: "Classes en ligne (visioconférence)"
resume: "Une classe en ligne est une séance de cours à distance (visioconférence) programmée pour une classe et une matière, à une période donnée."
audiences: [school_admin, teacher]
---
# 💻 Classes en ligne (visioconférence)

## 🎯 Rôle
Une **classe en ligne** est une **séance de cours à distance** (visioconférence) programmée
pour une **classe** et une **matière**, à une **période** donnée. L'enseignant **ouvre la
session**, les élèves **rejoignent le lien**, et le cours se déroule en direct. Ce module
gère le **planning et le lancement** de ces séances.

## ✅ Prérequis
1. Avoir **classes, matières, enseignants** et une **période/emploi du temps** (*01*).
2. Option « Online Class » + permissions.
3. Accès : menu **Online Class** (`online-class.index`).

## 🟢 Programmer une classe en ligne (étape par étape)
1. Ouvrez **Online Class** → **« Ajouter »**.
2. Renseignez :
   - la **Classe / section** ;
   - la **Matière** (liste dynamique `online-class.subjects`) ;
   - la **Période / créneau** (`online-class.periods`) — date + heure ;
   - l'**enseignant** et, selon le cas, un **lien/salle** de visio.
3. **Enregistrez** (`online-class.store`). La séance apparaît dans le **planning**.

## ▶️ Lancer / rejoindre une séance
1. Ouvrez la **liste des séances** (`online-class.show`).
2. Le jour dit, l'enseignant **démarre** la classe et **partage le lien** ; les élèves
   **rejoignent** la visio (depuis le web ou l'app).

## ✏️ Modifier une séance
1. Sur la séance, **Modifier** → `online-class.update` : changez période, classe, matière ou
   enseignant (ex. **report** d'un cours).

## 🔴 Supprimer une séance
1. Icône **Supprimer** (`online-class.destroy`), confirmez → la séance est **retirée** du
   planning.

## ♻️ Restaurer
- ⚠️ Les **classes en ligne ne sont pas restaurables** : une séance supprimée se **recrée**
  (`online-class.store`). Pour un simple **report**, **modifiez** la période plutôt que de
  supprimer.

## ⚠️ Bon à savoir
- **Période ≠ emploi du temps fixe** : une classe en ligne est une **séance ponctuelle** ;
  planifiez-la en cohérence avec l'emploi du temps (*01*).
- **Prévenez les élèves** (annonce/notification, PARTIE Présences-Communication) avec le
  **lien** et l'**heure**.
- **Testez le lien/la caméra** avant l'heure pour éviter les temps morts.
- Le **module homework/cours** (*03*, *04*) reste la mémoire des **contenus** ; la classe en
  ligne est le **direct**.
- Accès **réservé** aux personnes de la classe : ne diffusez pas publiquement le lien.
