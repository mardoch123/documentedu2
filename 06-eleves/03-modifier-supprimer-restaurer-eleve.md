---
id: 06-03-modifier-supprimer-restaurer-eleve
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-03-modifier-supprimer-restaurer-eleve
emoji: "✏️"
titre: "Modifier, désactiver, supprimer et retrouver un élève"
resume: "Cette page rassemble tout le cycle de vie d'une fiche élève après son admission : corriger une information, mettre un élève « en veille » (désactivation), le supprimer, et surtout le retrouver en c..."
audiences: [school_admin, staff]
---
# ✏️ Modifier, désactiver, supprimer et retrouver un élève

## 🎯 Rôle
Cette page rassemble **tout le cycle de vie** d'une fiche élève après son admission :
corriger une information, mettre un élève « en veille » (désactivation), le supprimer, et
surtout **le retrouver** en cas d'erreur. C'est la page à lire avant de toucher à un élève
existant, pour ne jamais perdre de données par mégarde.

## ✅ Prérequis
1. L'élève existe déjà (voir *02-admettre-un-eleve.md*).
2. Permissions : « student-edit » (modifier), « student-delete » (désactiver/supprimer).
3. Accès : menu **Élèves → Info Apprenant**.

## ✏️ Modifier une information (le plus courant)
1. Ouvrez **Élèves → Info Apprenant**.
2. **Recherchez** l'élève (case de recherche : tapez 2-3 lettres de son nom).
3. Deux façons de modifier :
   - **Crayon ✏️** directement sur la ligne, ou
   - **Clic sur le nom** de l'élève → panneau d'actions → **Modifier**.
4. L'assistant d'inscription se rouvre **pré-rempli**. Allez à l'étape concernée
   (Identité, Parent, etc.) et corrigez uniquement le champ fautif.
5. Cliquez sur **Mettre à jour / Soumettre**.
6. Vérifiez dans la liste que la correction est bien prise en compte.
> Exemples fréquents : orthographe du nom, mauvais numéro de parent, changement de classe,
> photo à ajouter, email à remplacer par un vrai.

## 🔴 Les DEUX façons de « retirer » un élève (à bien distinguer)

### A) Désactiver = mettre en veille (RÉVERSIBLE — à privilégier)
Un élève désactivé quitte la liste des élèves « actifs » mais **conserve** ses notes,
présences et paiements. C'est ce qu'on fait pour un départ, un redoublement, un doublon.
1. Cochez la **case** de l'élève dans la liste (ou plusieurs d'un coup).
2. Le bouton **« Inactive »** au-dessus de la liste devient cliquable → cliquez dessus.
3. Confirmez. L'élève bascule dans l'onglet **« Inactive »**.

### B) Supprimer = retirer du logiciel (QUASI IRRÉVERSIBLE)
1. Soit la **poubelle 🗑** sur la ligne, soit bouton **« Supprimer la sélection »** après
   avoir coché les élèves.
2. Fenêtre de confirmation → **OK**.
⚠️ **Un élève supprimé ne se restaure pas depuis cet écran** (pas de corbeille élève comme
pour les classes). Ses données ne sont plus accessibles par vous. En cas de suppression
accidentelle : **contactez immédiatement le Support EduEasy** qui pourra la rétablir côté
serveur. **Ne supprimez jamais pour « corriger » : désactivez.**

## ♻️ Retrouver / réactiver un élève désactivé
1. En haut de **Info Apprenant**, cliquez sur l'onglet **« Inactive »** (à côté de « active »).
2. Recherchez l'élève (mêmes outils de recherche que la liste active).
3. Cochez sa case → le bouton devient **« Active »** → cliquez → confirmez.
4. Retournez sur **« active »** : l'élève est revenu **avec tout son historique intact**
   (bulletins, paiements, présences d'avant).

## ⚠️ Bon à savoir
- **Règle d'or** : pour enlever un élève, on **désactive** ; on ne **supprime** que sur
  instruction explicite (doublon_created_par_erreur sans aucune donnée derrière).
- Un élève **désactivé compte toujours** dans certaines statistiques d'année : c'est voulu,
  pour que les totaux de l'année restent justes.
- **Changement de classe en cours d'année** : passez par Modifier (étape 1 « Affectation »),
  ne recréez pas la fiche — sinon l'élève perd ses notes déjà saisies.
- La **réactivation est instantanée** ; faites-la devant le parent si besoin pour lui
  montrer que le compte remarche.
