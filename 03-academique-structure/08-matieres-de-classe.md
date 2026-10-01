---
id: 03-08-matieres-de-classe
partie: 3
titre_partie: "Académique : Structure & Matières"
app: web
slug: 03-08-matieres-de-classe
emoji: "📘"
titre: "Les Matières de classe (Class Subject)"
resume: "Cette page affecte les matières du référentiel à une classe précise : « Mathématiques est enseignée en 6ème A », « Sport en Terminale C »…"
audiences: [school_admin]
---
# Les Matières de classe (Class Subject)

## 🎯 Rôle
Cette page **affecte les matières du référentiel à une classe précise** :
« Mathématiques est enseignée en 6ème A », « Sport en Terminale C »…
Sans cette étape, aucune matière n'apparaît dans les bulletins, les emplois du temps,
les saisies de notes ni les syllabus de la classe.

## ✅ Prérequis
1. Des **classes** créées → [07-classes.md](07-classes.md)
2. Des **matières** dans le référentiel → [03-matieres.md](03-matieres.md)
3. Permission « class-list » (le menu est le même que pour les classes).

Accès : menu **Académique → Class Subject** (ou lien « Matières de classe » depuis la page Classes).

## 🟢 Affecter une matière à une classe
1. Ouvrez **Class Subject**.
2. Cliquez sur le bouton **Ajouter / Créer** (formulaire en haut de page).
3. Choisissez dans les listes déroulantes :
   - la **Classe** (puis la **section** et le **semestre** demandés selon l'écran) ;
   - la **Matière** dans le référentiel ;
   - éventuellement le **type** (théorie/pratique) et le **coefficient/poids** si proposé.
4. Cliquez sur **Soumettre**.
5. La ligne apparaît dans la liste : « Classe – Matière – Section – Semestre ».
6. **Répétez l'opération pour chaque matière** de la classe (une soumission = une matière).
   💡 Travaillez matière par matière, classe par classe, pour ne pas vous perdre.

## ✏️ Modifier une affectation
1. Dans la liste, icône **crayon ✏️** sur la ligne concernée.
2. Changez la valeur voulue (classe, section, coefficient…) → **Soumettre**.

## 🔴 Supprimer une affectation
1. Icône **poubelle 🗑** sur la ligne → confirmer.
2. La matière disparaît **de cette classe uniquement** — elle reste dans le référentiel
   général et dans les autres classes.

⚠️ Ne supprimez pas une affectation contenant déjà des notes d'examen : vous perdriez
l'affichage de ces notes dans les bulletins de la classe.

## ♻️ Restaurer
L'affectation supprimée peut revenir via le filtre **« Trashed »** de la liste
si votre version l'active (icône **restaurer ♻️**) ; sinon, il suffit de **recréer
l'affectation à l'identique** (même classe, même matière, même section) : EduEasy
réaffiliera les données existantes.

## ⚠️ Bon à savoir
- Oublier cette étape est **la cause n°1** du message « aucune matière » quand on veut
  saisir des notes ou créer un emploi du temps.
- Pour vérifier rapidement ce qui manque : ouvrez la page **Syllabus** ou
  **Profs par matière** — les classes sans matières affectées y apparaissent vides.
