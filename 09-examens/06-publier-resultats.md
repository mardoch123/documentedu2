---
id: 09-06-publier-resultats
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-06-publier-resultats
emoji: "📤"
titre: "Publier (ou dépublier) les résultats d'un examen"
resume: "Publier un examen, c'est rendre officielles et visibles les notes des familles : le logiciel calcule alors les totaux, pourcentages, mentions et moyennes, enregistre les résultats et les affiche da..."
audiences: [school_admin]
---
# 📤 Publier (ou dépublier) les résultats d'un examen

## 🎯 Rôle
**Publier** un examen, c'est **rendre officielles et visibles** les notes des familles :
le logiciel **calcule alors les totaux, pourcentages, mentions et moyennes**, enregistre les
**résultats** et les **affiche** dans l'espace élève/parent. C'est le bouton qui fait « basculer »
un examen du statut « en préparation » au statut « résultats consultables ». Bonne nouvelle :
la publication est **réversible** (on peut **dépublier**).

## ✅ Prérequis
1. Avoir **saisi les notes de TOUTES les matières** de l'examen (*02* / *03*).
2. L'examen doit être **terminé** (statut « complet ») : sinon message
   *« Examen pas encore terminé »* ou *« Les notes ne sont pas encore téléchargées pour tous
   les sujets »*.
3. Avoir défini les **notations / mentions (grades)** pour l'échelle /20 (*09*).
4. Permission « exam-result ». Accès : menu **Offline Exam → Gérer les examens** ou
   **Résultat de l'examen publié** (`exams.get-result`).

## 🟢 Publier les résultats d'un examen (étape par étape)
1. Ouvrez **Gérer les examens** (`exams.index`).
2. **Cochez** la ou les lignes des examens prêts (case à gauche de chaque ligne).
3. Les boutons d'action de masse apparaissent en haut du tableau :
   - **« Publier la sélection (N) »** (bouton vert) → publie tous les examens cochés ;
   - pour un **seul** examen, utilisez plutôt l'**icône Publier** sur sa ligne.
4. Confirmez. Le logiciel **calcule** pour chaque élève : total, **pourcentage**, **moyenne
   /20**, **mention** (grade) et **statut admis/recomposé**, puis enregistre les résultats.
5. Une fois publié, les notes deviennent **visibles** des élèves et parents, et l'examen
   apparaît dans **« Résultat de l'examen publié »**.

## 🟡 Consulter un résultat publié
1. Menu **Offline Exam → Résultat de l'examen publié** (`exams.get-result`).
2. Sélectionnez **année scolaire + examen** pour afficher le **relevé des résultats**
   (moyennes, mentions, rangs), exportable/imprimable.

## 🔴 Dépublier (revenir en arrière)
1. Retournez dans **Gérer les examens**.
2. **Cochez** l'examen déjà publié.
3. Cliquez **« Dépublier la sélection (N) »** (bouton orange), ou l'**icône Dépublier** sur la
   ligne pour un seul examen.
4. ⚠️ **Dépublier supprime les résultats calculés** de cet examen et **remet les notes « non
   publiées »** : les familles ne les voient plus. Vous pouvez alors corriger les notes (*02*)
   et **re-publier**.

## ♻️ Restaurer des résultats
- **Re-publier** l'examen (*🟢 ci-dessus*) **recalcule et restaure** les résultats : la
  publication/dépublication est un **interrupteur**, sans corbeille.
- L'**examen** lui-même, si supprimé, se restaure via l'onglet **« Trashed »** (*01*) — mais
  on ne peut pas supprimer définitivement un examen dont les notes sont publiées.

## ⚠️ Bon à savoir
- **Toutes les matières ou rien** : la publication refuse tant qu'il manque une matière ;
  complétez d'abord la saisie.
- **Vérifiez avant de publier** : la publication envoie les résultats aux familles ; faites un
  contrôle dans **Notes non publiées** (*05*) d'abord.
- **Moyenne sur 20** : le pourcentage est converti en note /20 puis en **mention** selon le
  barème que vous avez configuré (*09-notations-grades.md*).
- **Dépublier n'efface pas les notes saisies** : elles restent ; seuls les **résultats
  publiés** sont retirés. Vous pouvez publier à nouveau sans tout ressaisir.
- Les **bulletins** (*07*) utilisent les résultats publiés : publiez avant de générer un
  bulletin.
