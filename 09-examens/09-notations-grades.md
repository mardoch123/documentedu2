---
id: 09-09-notations-grades
partie: 9
titre_partie: "Examens, bulletins & évaluations"
app: web
slug: 09-09-notations-grades
emoji: "🏅"
titre: "Notations & mentions (barèmes de notes / grades)"
resume: "Les grades (ou notations / mentions) définissent le barème qui transforme une moyenne chiffrée en appréciation : par ex."
audiences: [school_admin]
---
# 🏅 Notations & mentions (barèmes de notes / grades)

## 🎯 Rôle
Les **grades** (ou **notations / mentions**) définissent le **barème** qui transforme une
**moyenne chiffrée** en **appréciation** : par ex. « 10–11,99 → Passable »,
« 16–20 → Très Bien ». Ces plages servent partout : **publication des résultats** (*06*),
**bulletins** (*07*), **moyennes de passage** (*08*). Cette page permet de **créer, générer
par défaut, modifier et supprimer** ces plages, organisées **par pays et par cycle**.

## ✅ Prérequis
1. Permission « grade-create ».
2. Avoir choisi le **pays** et le **cycle** concernés (le barème en dépend).
3. Accès : menu **Offline Exam → Notation / exam_grade** (`exam.grade.index`).

## 🟢 Créer / configurer un barème de mentions
1. Ouvrez **Notation** (sous-titre : *« Définissez les barèmes de notes par pays et par
   cycle, avec génération des plages par défaut. »*).
2. Sélectionnez :
   - **« country »** (pays) — ex. **Bénin**, **Guinée**, etc. ;
   - **« cycle »** — **Primaire**, **Collège**, **Lycée**.
3. Le plus simple : cliquez **« generate_default_grades »** (Générer les plages par défaut).
   Le logiciel **remplit automatiquement** les plages selon le pays + cycle choisis
   (ex. Collège/Lycée Bénin : 0–9,99 Échec · 10–11,99 Passable · 12–13,99 Assez Bien ·
   14–15,99 Bien · 16–20 Très Bien).
4. Pour **ajouter une ligne manuellement**, cliquez **« add_new_data »** et remplissez :
   - **« starting_range »** ★ — note de **début** de la plage (0 à 20) ;
   - **« ending_range »** ★ — note de **fin** de la plage (0 à 20) ;
   - **« grade »** ★ — la **mention** correspondante (texte libre : « Excellent », « Bien »…).
5. Cliquez **« submit »** pour **enregistrer tout le barème**.

## ✏️ Modifier une plage
1. Revenez sur la page **Notation**, re-choisissez le pays + cycle.
2. Les plages existantes s'affichent : changez les **bornes** ou le **libellé de mention**.
3. **Submit** pour ré-enregistrer.

## 🔴 Supprimer une plage / tout effacer
- Pour **retirer une seule plage**, cliquez la **croix (✕)** à droite de sa ligne (suppression
  de ligne), puis **submit**.
- Pour **partir de zéro**, cliquez **« clear_all »** (Clear all) : **toutes les plages** de la
  configuration courante sont **vidées**, puis vous **re-générez** ou **re-saisissez**.

## ♻️ Restaurer un barème
- Il n'y a **pas de corbeille** pour les mentions : si vous effacez par erreur, cliquez à
  nouveau **« generate_default_grades »** pour **restaurer les plages par défaut** du pays +
  cycle, puis complétez.
- Notez vos **barèmes personnalisés** ailleurs : une fois « clear_all », ils ne sont pas
  récupérables automatiquement.

## ⚠️ Bon à savoir
- Le barème est **sur 20** (champs bornés 0 → 20) : c'est l'échelle utilisée pour convertir
  les pourcentages en note et en mention.
- **Un barème par pays + cycle** : adaptez-le au règlement de votre établissement ; les
  collégiens/lycéens n'ont pas les mêmes seuils que le primaire.
- Sans mentions configurées, la **publication** peut échouer (message « Les données de notes
  n'existent pas ») : **configurez d'abord les grades**.
- Les **bornes ne doivent pas se chevaucher** et doivent **couvrir toute l'échelle** (0 à 20)
  pour qu'une moyenne tombe toujours dans une plage.
