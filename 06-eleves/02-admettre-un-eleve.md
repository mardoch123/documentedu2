---
id: 06-02-admettre-un-eleve
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-02-admettre-un-eleve
emoji: "🧾"
titre: "Admettre un élève (créer une fiche, pas à pas)"
resume: "C'est le formulaire d'inscription."
audiences: [school_admin, staff]
---
# 🧾 Admettre un élève (créer une fiche, pas à pas)

## 🎯 Rôle
C'est le **formulaire d'inscription**. Il remplace la fiche papier : vous saisissez l'élève
en **5 étapes guidées** (un « assistant » qui avance étape par étape), et à la fin le
logiciel crée la fiche, l'identifiant de connexion et (si vous le demandez) le mot de passe
du parent. Une seule saisie, tout le reste de l'année s'en suit.

## ✅ Prérequis
1. Avoir créé la **classe / section** qui recevra l'élève (*Structure académique → Classes*).
2. Avoir défini l'**année de session** courante (*Académique → Année/session*).
3. Avoir au moins un **médium** et une **filière** si votre école les utilise.
4. Permission « student-create ».
5. Accès : menu **Élèves → Admission** (icône 👤+).

## 🟢 Les 5 étapes d'une admission (étape par étape)

### Étape 1 — Affectation Scolaire & Conditions
1. Choisissez la **Classe / Section** de l'élève (liste déroulante ★ obligatoire).
2. Sélectionnez l'**année de session**, le **médium**, la **filière** et la **section** si demandés.
3. Renseignez les éventuelles **conditions d'inscription** demandées par votre école
   (dates, statut, mode d'entrée…).
4. Cliquez sur **« Étape suivante : Profil Apprenant »**.

### Étape 2 — Identité de l'Apprenant
1. Saisissez le **Prénom** ★, le **Nom** ★, le **Sexe** (boutons 👦/👩), la **date de naissance**.
2. Ajoutez les infos secondaires utiles : lieu de naissance, nationalité, adresse…
3. **Photo** : cliquez sur la zone photo pour téléverser le portrait (facultatif à cette étape,
   mais fortement conseillé — voir aussi la page *07-telecharger-photos-eleves.md* pour en masse).
4. **« Étape suivante »**.

### Étape 3 — Renseignements Complémentaires
- Cette étape affiche **les champs supplémentaires définis par votre école** (case « Oui/Non »,
  classes de transport, régime alimentaire, etc.). Elle peut être absente si votre école n'a
  créé aucun champ complémentaire.
- Remplissez ce qui concerne l'élève, puis **« Étape suivante »**.

### Étape 4 — Responsable Légal / Parent
1. Le logiciel vous propose deux modes (onglets) :
   - **Rechercher un parent existant** : si un autre élève de l'école a déjà le même parent,
     tapez son nom et **sélectionnez-le** → vous ne ressaisissez rien.
   - **Créer un nouveau parent** : remplissez Prénom ★, Nom ★, Email ★, Mobile ★, Sexe ★,
     (photo facultative).
2. **Case « Générer automatiquement l'email »** : cochez-la si le parent **n'a pas d'adresse
   email réelle** → le système fabriquera un identifiant du type `eleve@edueasy.net` pour que
   le parent puisse se connecter à l'application. Décochez-la pour saisir un vrai email.
3. Renseignez le **lien de parenté** (Père, Mère, Tuteur…).
4. **« Étape suivante »**.

### Étape 5 — Récapitulatif & Confirmation
1. **Relisez tout le récapitulatif** : classe, identité, parent. C'est votre dernier contrôle.
2. Cliquez sur **Soumettre / Enregistrer**.
3. Un message de succès apparaît ; l'élève figure désormais dans **Élèves → Info Apprenant**.
4. Notez/communiquez l'**identifiant** (email généré ou saisi) créé pour le compte élève/parent.

## ✏️ Modifier une fiche après admission
1. **Élèves → Info Apprenant** → cliquez sur le nom de l'élève → **Modifier** (crayon ✏️).
2. Le même assistant se rouvre **pré-rempli** ; corrigez l'étape qui convient.
3. **Mettre à jour**. (Ne recréez jamais un élève qui existe déjà : modifiez-le.)

## 🔴 Annuler une admission erronée
- Si l'élève vient d'être créé et n'a encore **aucune note ni paiement** :
  **Élèves → Info Apprenant** → cochez sa case → bouton **« Inactive »** (désactivation
  réversible). Voyez la page *01-liste-et-fiche-eleve.md* pour la différence
  désactiver / supprimer.
- Évitez la **suppression définitive** (poubelle) : un élève supprimé n'est pas restaurable
  depuis ce module.

## ♻️ Retrouver / réactiver un élève mal désactivé
1. **Élèves → Info Apprenant** → onglet **« Inactive »**.
2. Cochez l'élève → bouton **« Active »** → confirmez. Il revient avec tout son historique.

## ⚠️ Bon à savoir
- **Cherchez avant de créer** : tapez le nom dans la liste des élèves pour éviter les doublons
  (un même élève admis deux fois fausse les présences et les finances).
- Les champs marqués **★** (astérisque rouge) sont **obligatoires** : sans eux, l'étape refuse
  d'avancer.
- Vous pouvez avancer/reculer entre les étapes avec **« Étape précédente »** sans rien perdre.
- L'**email généré** (badge « Généré ») sert uniquement de compte de connexion ; le vrai contact
  reste le **mobile** du parent — mettez un numéro valide (WhatsApp/SMS en dépendent).
- Pour **plusieurs élèves à la fois**, préférez l'ajout en masse (*06-ajout-en-masse.md*) ou
  l'**Import Intelligent IA** plutôt que de refaire 30 fois ce formulaire.
