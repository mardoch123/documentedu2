---
id: 04-02-bascule-annee
partie: 4
titre_partie: "Académique : Outils IA"
app: web
slug: 04-02-bascule-annee
emoji: "📘"
titre: "Bascule d'Année en 1 clic (Auto Rollover)"
resume: "Le saut de fin d'année : tous les élèves montent d'une classe (6ème → 5ème), les classes de sortie sont archivées, les nouveaux semestres sont créés, les affectations de professeurs sont reconduites."
audiences: [school_admin]
---
# Bascule d'Année en 1 clic (Auto Rollover)

## 🎯 Rôle
Le **saut de fin d'année** : tous les élèves montent d'une classe (6ème → 5ème),
les classes de sortie sont archivées, les nouveaux semestres sont créés, les
affectations de professeurs sont reconduites. Une seule opération au lieu de 3 heures
de travail manuel.

## ✅ Prérequis (à vérifier AVANT de lancer)
1. La **nouvelle année scolaire (session)** doit exister :
   *Paramètres de l'Établissement → Année Scolaire → Créer* (ex. `2026-2027`).
2. Les **classes de destination** doivent exister pour l'année suivante ou être créées
   par l'outil si proposé (une « Terminale » qui sort n'a pas de destination : normal).
3. Les **dernières notes** de l'année en cours doivent être saisies et publiées.
4. Idéalement : faire une **sauvegarde** d'abord
   (*Sauvegarde de la base* ou *Paramètres → Points de Restauration*).
5. Accès : menu **Académique → Bascule d'Année (1 Clic)**.

## 🟢 Lancer la bascule (étape par étape)
1. Ouvrez **Bascule d'Année**.
2. Sélectionnez l'**année source** (qui se termine) et l'**année destination**.
3. L'outil affiche le **plan de promotion** : pour chaque classe, la classe suivante
   automatique (modifiable : vous pouvez changer la destination classe par classe).
4. Choisissez le **sort des élèves non promus** : redoublants à garder dans la même
   classe, élèves sortants à désactiver.
5. Cochez les options souhaitées : recréer les semestres, reconduire les profs,
   réinitialiser les présences, etc.
6. Cliquez sur **Aperçu / Simuler** si disponible : un rapport montre ce qui VA être fait
   sans rien modifier.
7. Cliquez sur **Lancer la bascule** puis **Confirmer**.
8. Attendez la fin du traitement (les élèves nombreux peuvent prendre plusieurs minutes ;
   ne fermez pas la page). Un rapport de résultat s'affiche.

## ✏️ Corriger après la bascule
La bascule crée des situations normales, donc tout se corrige dans les modules standards :
- un élève mal placé → *Élèves → modifier sa fiche* (changer classe/section) ;
- une classe manquante → *Académique → Classes → créer* ;
- un redoublant raté → remplacer sa classe destination dans sa fiche élève.

## 🔴 Annuler une bascule (supprimer ses effets)
⚠️ Il n'existe **pas de bouton « annuler la bascule »** : c'est une opération engageante.
Deux solutions seulement :
1. **Restaurer le point de sauvegarde** créé juste avant
   (*Paramètres → Points de Restauration → Restaurer*) — propre et total ;
2. Ou corriger manuellement classe par classe (long).
**C'est pour cela que la sauvegarde préalable est obligatoire dans la procédure.**

## ♻️ Bonne pratique de « restauration »
Si la bascule a été lancée trop tôt (examens pas finis) : revenez en arrière via le point
de restauration, terminez l'année, puis relancez la bascule. Après restauration, vérifiez
le tableau de bord (chiffres d'élèves) et une ficheélève prise au hasard.

## ⚠️ Bon à savoir
- Lancez la bascule **en dehors des heures d'affluence** (tard le soir) : pendant
  l'opération, les écrans élèves peuvent être incohérents.
- Les **frais impayés** de l'ancienne année restent attachés à l'élève : c'est voulu,
  les recouvrements continuent (voir Lettrage & Reçus IA).
- Les classes de sortie (ex. Terminale) ne sont pas supprimées : elles deviennent
  simplement « vides » pour la nouvelle année.
