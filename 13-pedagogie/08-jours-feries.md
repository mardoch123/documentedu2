---
id: 13-08-jours-feries
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-08-jours-feries
emoji: "📅"
titre: "Jours fériés (Holiday List) & Cahiers de Vacances IA"
resume: "Ce module gère le calendrier des jours fériés / vacances de l'école : chaque période de fermeture (nom, date de début, date de fin) est déclarée pour que l'emploi du temps, les présences et les app..."
audiences: [school_admin]
---
# 📅 Jours fériés (Holiday List) & Cahiers de Vacances IA

## 🎯 Rôle
Ce module gère le **calendrier des jours fériés / vacances** de l'école : chaque **période de
fermeture** (nom, date de début, date de fin) est déclarée pour que l'emploi du temps, les
présences et les applications mobiles **sachent qu'il n'y a pas cours**. Il est complété par
les **Cahiers de Vacances IA** : un **cahier de travail** généré automatiquement pour chaque
élève à faire **pendant les vacances**, téléchargeable en PDF et **envoyé par notification**.

## ✅ Prérequis
1. Avoir **classes, sections et élèves**.
2. Abonnement avec la fonction **« Holiday Management »** (jours fériés).
3. Permissions « holiday-* ». Accès : menu **Holiday List** (`holiday.index`).
4. Pour les **cahiers de vacances** : accès **Cahiers de Vacances IA**
   (`holiday-workbooks.index`), outil **IA payant**.

## 🟢 Déclarer un jour férié (étape par étape)
1. Ouvrez **Holiday List** → **« Ajouter »**.
2. Renseignez :
   - **Titre / nom** du jour férié (ex. : *Fête de l'Indépendance*) ;
   - **Date de début** (`start_date`) et **date de fin** (`end_date`) ;
   - **Remarque / description** éventuelle.
3. **Enregistrez** (`holiday.store`). La période est **marquée « pas cours »** partout.

## 📘 Générer les Cahiers de Vacances IA (étape par étape)
1. Ouvrez **Cahiers de Vacances IA** (`holiday-workbooks.index`).
2. Choisissez les **élèves / classes** concernés.
3. Lancez la génération :
   - **par lot** pour toute une classe (`holiday-workbooks.generate-batch`) ;
   - **pour un seul élève** (`holiday-workbooks.generate-single/{studentId}`).
4. L'IA compose un **cahier de travail** adapté (exercices de révision).
5. **Téléchargez le PDF** (`holiday-workbooks.download/{id}`) pour impression/remise.
6. **Renvoyer la notification** aux parents/élèves si besoin
   (`holiday-workbooks.resend/{id}`) ; l'élève récupère aussi via le **lien public sécurisé**
   (`holiday-workbooks.public-download` par jeton).

## ✏️ Modifier un jour férié
1. Icône **Modifier** (`holiday.edit`) → corrigez titre/dates → `holiday.update`.

## 🔴 Supprimer un jour férié
1. Icône **Supprimer** (`holiday.destroy`), confirmez → la période **disparaît**.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** : un jour férié supprimé se **recrée** simplement (saisie courte).
- Les **cahiers de vacances** déjà **générés/téléchargés** restent valables : relancez une
  génération si vous voulez une nouvelle version.

## ⚠️ Bon à savoir
- **Déclarez les vacances tôt** : l'emploi du temps et les apps mobiles en tiennent compte.
- **Chevauchement de dates** : évitez de créer deux périodes qui se recouvrent.
- **Cahiers IA = payant** : chaque génération **consomme des crédits** ; visez les lots.
- Le **lien public** du cahier est **sécurisé par jeton** : partagez-le seulement avec les
  parents concernés.
- Les catégories de *07-cahier-etudiant.md* (cahier journal) sont **différentes** : ici il
  s'agit du **calendrier** et du **travail de vacances**, pas des observations d'élèves.
