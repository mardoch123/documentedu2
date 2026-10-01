---
id: 16-03-app-mobile-edustaff
partie: 16
titre_partie: "Vues Enseignant, Staff et mobiles"
app: web
slug: 16-03-app-mobile-edustaff
emoji: "📱"
titre: "L'application mobile EduStaff (profs & personnel)"
resume: "- Permettre à un enseignant de gérer sa classe depuis la salle de cours : appel, leçons données, devoirs, notes, emploi du temps."
audiences: [school_admin, teacher, staff]
---
# 📱 16.3 — L'application mobile EduStaff (profs & personnel)

EduStaff est l'**application pour téléphone** (Android et iPhone) destinée aux
**enseignants et au personnel** de l'école. Elle donne accès aux mêmes informations que
le site EduEasy, mais dans la poche : faire l'appel en classe, saisir une note, envoyer un
message, consulter sa paie… sans ordinateur.

## 🎯 Rôle
- Permettre à un enseignant de gérer sa classe **depuis la salle de cours** :
  appel, leçons données, devoirs, notes, emploi du temps.
- Permettre au personnel de consulter **ses informations RH** : congés, paie, documents,
  annonces — et d'accomplir les tâches que la direction a autorisées.
- Tout ce qui est saisi dans l'application apparaît **immédiatement sur le web**
  (même serveur), et inversement.

> 📖 **Cette page est un aperçu.** Le **pas à pas complet, écran par écran** (29 pages,
> PARTIE 17 du sommaire) se trouve dans le dossier
> [17-app-edustaff](../17-app-edustaff/01-installer-et-se-connecter.md) :
> [installation et connexion](../17-app-edustaff/01-installer-et-se-connecter.md) ·
> [accueil selon rôle](../17-app-edustaff/02-accueil-selon-role.md) ·
> [appel des élèves](../17-app-edustaff/07-appel-des-eleves.md) ·
> [encaissement des frais](../17-app-edustaff/20-encaissement-frais.md) ·
> [profil et déconnexion](../17-app-edustaff/29-profil-et-divers.md).

## ✅ Prérequis
- Que l'école utilise EduEasy (l'application se connecte au compte de l'école).
- Avoir un **compte enseignant ou personnel** créé par la direction (voir pages 16.1
  et 16.2) : l'application refuse un compte élève.
- Télécharger l'application « EduStaff » sur le Play Store (Android) ou l'App Store
  (iPhone), et connaître l'adresse / le code de son école demandés à l'écran de connexion.
- Internet sur le téléphone (3G/4G/Wi-Fi).

## 🟢 Installer et se connecter
1. Installez EduStaff depuis le store de votre téléphone.
2. Ouvrez l'application : l'écran de connexion demande vos **identifiants de l'école**
   (mobile ou e-mail + mot de passe), et éventuellement le nom/code de l'école.
3. Appuyez sur « Se connecter ». L'accueil s'affiche avec vos menus.
4. **Important** : acceptez la demande « Autoriser les notifications » pour recevoir
   les annonces de la direction et les alertes de paie/congés en temps réel (Firebase).
5. En cas de refus de connexion répété, utilisez « Mot de passe oublié » ou appelez le
   secrétariat de l'école : le compte appartient à l'école, pas à vous.

## 📚 Les grandes fonctions de l'application
Les écrans dépendent de vos **autorisations** : l'application masque d'elle-même ce que
vous n'avez pas le droit de faire (règle identique au web).
- **Mes classes** : listes de vos classes/sections et de vos élèves avec photo.
- **Faire l'appel** : cocher Présent / Absent / Retard élève par élève pour la séance du
  jour, puis valider. Les absences déclenchent les notifications prévues par l'école.
- **Mes leçons / plan de cours** : consulter le programme et **pointer (lettrer)** la
  leçon effectivement donnée.
- **Devoirs** : créer un devoir (titre, consigne, date, classe), puis **corriger et saisir
  les notes** remis par les élèves.
- **Résultats** : consulter les notes et moyennes de ses élèves ; saisie des notes
  d'évaluation selon les droits.
- **Emploi du temps** : ses cours du jour et de la semaine, avec salles et classes.
- **Congés** : poser une demande de congé (dates + motif) et suivre sa validation.
- **Ma paie** : consulter ses fiches de paie et accusés de réception.
- **Mon profil / mes documents** : photo, coordonnées, pièces de son dossier RH.
- **Messagerie interne & annonces** : chat avec le personnel autorisé et affichage des
  annonces de la direction.

## ✏️ Modifier
- Une présence, une note ou un devoir **se modifie depuis l'application comme depuis le
  web** : ouvrez l'élément, changez la valeur, enregistrez. La version la plus récente
  enregistrée gagne (évitez de travailler à deux dessus en même temps).
- **Photo du profil** : Profil → toucher la photo → choisir une image → valider.
- **Mot de passe** : Profil → changer le mot de passe (identique au web).

## 🔴 Supprimer
- Dans l'application : un devoir ou une leçon créée se supprime par son bouton
  « Supprimer » (confirmé par une question « êtes-vous sûr ? »).
- **On ne supprime jamais son propre compte** depuis l'application : le compte est géré
  par la direction sur le web (menu « Personnel »).
- Désinstaller l'application **n'efface aucune donnée** : tout reste sur le serveur de
  l'école, il suffit de réinstaller et de se reconnecter.

## ♻️ Restaurer
- Il n'y a **pas de corbeille dans l'application** : un élément supprimé de l'app est
  supprimé comme si vous l'aviez fait du web. Selon les modules, une restauration est
  possible **depuis le site web** (corbeille du menu « Personnel », archives élève…), sinon
  il faut **recréer l'élément** (nouveau devoir, nouvel appel à refaire).
- En cas de fausse manipulation importante (gros appel effacé), prévenez la direction :
  elle peut ressaisir ou corriger depuis le web avec ses pleins droits.

## ⚠️ Bon à savoir
- L'application affiche toujours **les mêmes données que le web** : aucune donnée
  « téléphone » séparée, pas de double saisie.
- Les menus manquants = autorisations manquantes : à demander à la direction, pas un bug.
- Gardez l'application à jour (store) : les nouvelles fonctions d'EduEasy y arrivent par
  mise à jour, comme sur le web.
- Notifications push : si vous ne recevez plus les annonces, vérifiez dans les réglages du
  téléphone que les notifications d'EduStaff sont bien autorisées.
- Perte de téléphone : prévenez la direction ; personne ne peut lire vos données depuis
  l'appareil perdu tant que vous n'y êtes pas reconnecté, et la direction peut changer vos
  accès.
