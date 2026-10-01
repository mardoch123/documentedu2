---
id: 05-01-promouvoir-transférer-eleves-interne
partie: 5
titre_partie: "Académique : Mobilité"
app: web
slug: 05-01-promouvoir-transférer-eleves-interne
emoji: "📘"
titre: "Promouvoir et transférer des élèves (à l'intérieur de l'école)"
resume: "Deux opérations jumelles dans le module « Transfer & Promote Students » : - Promouvoir : faire monter un élève d'un niveau (6ème → 5ème) en fin d'année ; - Transférer (changement"
audiences: [school_admin]
---
# Promouvoir et transférer des élèves (à l'intérieur de l'école)

## 🎯 Rôle
Deux opérations jumelles dans le module **« Transfer & Promote Students »** :
- **Promouvoir** : faire monter un élève d'un niveau (6ème → 5ème) en fin d'année ;
- **Transférer (changement interne)** : déplacer un élève d'une classe/section à une autre
  (6ème A → 6ème B), ou le changer de statut (redoublement).

## ✅ Prérequis
1. La **classe de destination** doit exister
   ([07-classes.md](../03-academique-structure/07-classes.md)).
2. Permission « promote-student-create » ou « transfer-student-create ».
3. Accès : menu **Académique → Transfer & Promote Students**.

## 🟢 Promouvoir un ou plusieurs élèves
1. Ouvrez **Transfer & Promote Students**.
2. Sélectionnez la **classe d'origine** (ex. 6ème A) dans les filtres.
3. La liste des élèves apparaît avec leurs cases à cocher :
   - cochez les élèves **un par un** (les promus) ;
   - ou « Tout sélectionner » pour toute la classe.
4. Choisissez la **classe/section de destination** (ex. 5ème A) et le nouvel
   **année/semestre** si demandé.
5. Pour les **redoublants** : ne les cochez pas ici — passez plutôt par « Transférer »
   vers la même classe d'origine (6ème A version nouvelle année).
6. Cliquez sur **Promouvoir / Valider**.
7. Le récapitulatif affiche le nombre d'élèves déplacés ; vérifiez-les dans la liste
   des élèves de la classe destination.

## 🟢 Transférer un élève entre classes/sections (changement interne)
1. Même page, onglet ou bouton **Transfert interne / Change Class**.
2. Choisissez l'**élève** (recherche par nom ou matricule).
3. Sélectionnez la **nouvelle classe et section** + le motif si un champ existe
   (ex. « répartition équilibrée », « demande parent »).
4. Cliquez sur **Transférer / Valider**.
5. L'élève disparaît de l'ancienne liste et apparaît dans la nouvelle, **avec son historique**
   (notes, présences de l'ancienne classe conservées).

## ✏️ Annuler / corriger une promotion ou un transfert
1. Retournez dans le module, retrouvez l'élève (filtre par nom).
2. Refaites l'opération dans le **sens inverse** (retransférez-le vers sa classe d'origine) :
   c'est la correction standard ; rien n'est perdu pendant le trajet.

## 🔴 Supprimer un élève promu par erreur
Si l'erreur est découverte après la bascule d'année : ne supprimez pas l'élève —
**modifiez sa fiche** (crayon ✏️ dans la liste des élèves) et replacez-le dans la bonne
classe, l'année et la section. La suppression (poubelle 🗑) est réservée aux doublons
créés par erreur.

## ♻️ Restaurer un élève supprimé après ces opérations
1. **Élèves → Liste** → filtre **« Trashed » / Corbeille**.
2. Icône **restaurer ♻️** sur sa ligne → il revient **avec sa dernière classe connues**.
3. Vérifiez et corrigez sa classe/section dans sa fiche si besoin.

## ⚠️ Bon à savoir
- Faites ces opérations **par petits groupes** (une classe à la fois) et vérifiez
  l'effectif affiché dans le tableau de bord après chaque gros mouvement.
- Les **numéros de matricule** peuvent être réattribués automatiquement dans la nouvelle
  classe (voir [03-numeros-matricules.md](03-numeros-matricules.md)).
- Un transfert change l'affichage des bulletins passés ? Non : les bulletins antérieurs
  gardent la classe d'origine — c'est normal et légalement nécessaire.
