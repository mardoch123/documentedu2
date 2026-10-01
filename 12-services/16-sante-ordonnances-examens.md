---
id: 12-16-sante-ordonnances-examens
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-16-sante-ordonnances-examens
emoji: "💊"
titre: "Santé : ordonnances et examens médicaux"
resume: "Après une consultation (15), le service santé peut rédiger une ordonnance (médicaments prescrits) et prescrire un examen médical (analyse, radio, test)."
audiences: [school_admin, staff]
---
# 💊 Santé : ordonnances et examens médicaux

## 🎯 Rôle
Après une **consultation** (*15*), le service santé peut **rédiger une ordonnance**
(médicaments prescrits) et **prescrire un examen médical** (analyse, radio, test). Ces deux
documents **s'archivent dans le dossier de l'élève**, se **consultent** à tout moment et —
pour l'ordonnance — **déclenchent la délivrance** de médicaments à la **pharmacie** (*17*).

## ✅ Prérequis
1. Avoir une **consultation** / un **dossier élève** (*15*).
2. Option « Health / Medical » + permissions santé.
3. Accès : menu **Health → Ordonnances** (`health.prescriptions.index`) et **Health →
   Examens** (`health.exams.index`).

## 📝 Rédiger une ordonnance (étape par étape)
1. Ouvrez **Ordonnances** → **« Nouvelle ordonnance »** (`health.prescriptions.create`).
2. Renseignez : l'**élève / la consultation** liée, les **médicaments prescrits**
   (nom, dosage, posologie, durée), la **date** et le **prescripteur**.
3. **Enregistrez** (`health.prescriptions.store`). L'ordonnance est **jointe au dossier**.
4. **Consulter** une ordonnance : `health.prescriptions.show` (et l'**imprimer** pour le
   parent/pharmacien).

## 🔬 Prescrire un examen médical (étape par étape)
1. Ouvrez **Examens** → **« Nouvel examen »** (`health.exams.create`, élève éventuellement
   **pré-sélectionné**).
2. Renseignez : l'**élève**, le **type d'examen** (analyse, imagerie, dépistage…), la
   **date**, le **motif** et le **résultat** quand il revient.
3. **Enregistrez** (`health.exams.store`). L'examen est **archivé dans le dossier**.
4. **Consulter** la liste : `health.exams.index`.

## ✏️ Compléter un résultat
- Un **examen** prescrit d'abord est **complété** avec son **résultat** lors du retour
  (réédition de la fiche d'examen) : on garde **prescription + résultat** ensemble.

## 🔴 Supprimer / ♻️ Restaurer
- ⚠️ **Ordonnances et examens sont des documents médicaux** : ils ne partent **pas à la
  corbeille**. On ne les **supprime** pas (intégrité du dossier) ; une erreur se **corrige
  par un nouveau document** ou un **complément** de résultat.
- L'**historique** des prescriptions/examens reste **consultable** dans le **dossier** de
  l'élève (*15*).

## ⚠️ Bon à savoir
- **Ordonnance → Pharmacie** : une ordonnance enregistrée permet au pharmacien de
  **délivrer** les médicaments correspondants (décrémente le stock, *17*).
- **Posologie claire** : précisez **dose, fréquence, durée** — c'est lu par des parents non
  soignants.
- **Allergies** : vérifiez le **dossier** (*15*) **avant** de prescrire (contre-indications).
- **Examens externes** : notez le **laboratoire / radiologue** et la **date de prélèvement**
  pour retrouver les résultats.
- Ces documents, comme tout le dossier santé, sont **confidentiels** : accès **restreint**.
