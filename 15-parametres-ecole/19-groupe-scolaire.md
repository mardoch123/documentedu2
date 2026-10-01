---
id: 15-19-groupe-scolaire
partie: 15
titre_partie: "Paramètres de l'établissement"
app: web
slug: 15-19-groupe-scolaire
emoji: "🏫"
titre: "Groupe scolaire : plusieurs écoles sous un même compte"
resume: "Vous dirigez plusieurs établissements (campus, antennes) ? Le groupe scolaire réunit vos écoles sous un seul compte direction : tableau comparatif des écoles (effectifs, paiement"
audiences: [school_admin]
---
# 🏫 Groupe scolaire : plusieurs écoles sous un même compte

## 🎯 Rôle
Vous dirigez **plusieurs établissements** (campus, antennes) ? Le **groupe scolaire** réunit
vos écoles sous **un seul compte direction** : **tableau comparatif** des écoles (effectifs,
paiements, indicateurs), **création/rattachement** d'écoles, **bascule instantanée** d'une
école à l'autre sans se déconnecter, et une **formule d'abonnement de groupe** avantageuse.

## ✅ Prérequis
1. Être **School Admin** d'une école **éligible groupe** (parlez-en au Support EduEasy pour
   l'activation/initiale mise en place).
2. Avoir la fonction **« Groupe scolaire »** à l'abonnement (`school-group.` routes,
   accessible hors enseignants).
3. Accès : menu **Groupe scolaire** (`school-group.index`).

## 🟢 Activer un groupe (étape par étape)
1. Ouvrez **Groupe scolaire** → **Activer le groupe** (`school-group.activate`).
2. Votre école actuelle devient la **mère** du groupe.
3. **Ajoutez les autres écoles** :
   - **créer une nouvelle école** dans le groupe (`school-group.schools.create`) — setup
     complet comme une nouvelle école ;
   - **rattacher une école existante** (`school-group.schools.attach`) — école déjà sur
     EduEasy que vous possédez (avec son accord/validation plateforme).

## 📊 Piloter le groupe
1. **Tableau comparatif** (`school-group.dashboard`) : écoles du groupe côte à côte —
   effectifs, paiements, modules utilisés.
2. **Basculer dans une école** (`school-group.switch/{school_id}`) : le menu, les classes,
   les frais deviennent **ceux de l'école choisie** — retour par le même sélecteur.
3. **Abonnement de groupe** (`school-group.subscription`) : formules spéciales (tarif
   dégressif par école, modules communs) — souscription comme *15*.

## ✏️ Modifier / 🔴 Détacher / ♻️ Restaurer
- Une école se **retire du groupe** par **détachement** (`school-group.schools.detach/{id}`) :
  elle **redevient autonome** (ses données lui restent). ⚠️ Confirmez avec le Support que
  l'école détachée garde son **abonnement propre** avant de détacher.
- **Restauration** : pour **re-rattacher** une école détachée → `schools.attach` à nouveau.
- Le groupe **ne se « supprime » pas** seul : passage par le Support EduEasy.

## ⚠️ Bon à savoir
- **Un seul login** pour tout le groupe : la **bascule remplace la déconnexion** — gagnez
  un temps énorme au moment des clôtures de fin d'année.
- **Les données ne se mélangent pas** : chaque école garde ses classes/élèves/frais ; le
  comparatif est une **lecture consolidée**, pas un pot commun.
- **Permissions** : un staff nommé dans une école **ne voit pas** les autres écoles.
- **Abonnement de groupe** : n'engagez le groupe que si toutes les écoles sont prêtes à
  **payer ensemble** (une école impayée dans le lot peut bloquer le renouvellement global).
- L'administration globale des groupes (côté équipe EduEasy) dépasse le cadre de ce guide :
  passez par le **Support** pour toute demande particulière sur le groupe.
