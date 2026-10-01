---
id: 06-05-reinitialiser-mots-de-passe-eleves
partie: 6
titre_partie: "Élèves"
app: web
slug: 06-05-reinitialiser-mots-de-passe-eleves
emoji: "🔑"
titre: "Réinitialiser les mots de passe des élèves"
resume: "Quand un élève (ou son parent) a oublié son mot de passe et cliqué sur « Mot de passe oublié ? » dans l'application mobile, une demande de réinitialisation arrive ici."
audiences: [school_admin, staff]
---
# 🔑 Réinitialiser les mots de passe des élèves

## 🎯 Rôle
Quand un élève (ou son parent) a **oublié son mot de passe** et cliqué sur « Mot de passe
oublié ? » dans l'application mobile, une **demande de réinitialisation arrive ici**. Vous la
voyez dans une liste, vous vérifiez l'identité, puis vous **redéfinissez un nouveau mot de
passe** que vous communiquez à la famille. C'est le « help-desk » des accès élèves.

## ✅ Prérequis
1. Permission « student-reset-password ».
2. L'élève doit avoir un compte (créé lors de l'admission).
3. Accès : menu **Élèves → Réinitialiser mots de passe** (icône 🔑).

## 🟢 Comment traiter une demande (étape par étape)
1. Ouvrez **Élèves → Réinitialiser mots de passe**.
2. Le bandeau du haut affiche le compteur **« Demandes en attente : X »** (nombre de familles
   bloquées). Un tableau « Comment ça marche » rappelle le principe en 3 cartes.
3. Dans la liste, repérez la demande (recherche possible par nom). Chaque ligne montre l'élève
   (avatar à initiales), sa date de naissance et la date de la demande.
4. Cliquez sur le bouton **« Réinitialiser »** de la ligne.
5. Le système redemande une **vérification d'identité** (généralement la **date de naissance**
   de l'élève) : saisissez-la pour prouver que vous êtes bien de l'école.
6. Un **nouveau mot de passe provisoire** s'affiche (ou est renvoyé au contact de l'élève).
7. **Communiquez ce mot de passe** à l'élève/parent (SMS, WhatsApp, de vive voix). Demandez-lui
   de le changer à sa première connexion.

## 🔁 Réinitialiser directement depuis la fiche d'un élève
Oui, sans attendre une demande :
1. **Élèves → Info Apprenant** → crayon **✏️** sur l'élève (ou clic sur son nom → Modifier).
2. Dans le formulaire d'édition, activez l'interrupteur **« reset_password »**
   (« Restaure le mot de passe initial de l'élève pour sa prochaine connexion »).
3. **Mettre à jour** : le mot de passe redevient celui par défaut, que vous transmettez.

## ✏️ / 🔴 Modifier ou annuler une réinitialisation
- Il n'y a rien à « modifier » : une réinitialisation est une action immédiate.
- Si vous vous êtes trompé d'élève, **réinitialisez le bon** ; l'ancien mot de passe provisoire
  cesse simplement de fonctionner à la prochaine connexion de l'autre compte.

## ⚠️ Bon à savoir
- **Ne partagez jamais le mot de passe par un canal non sécurisé** (ex. affiché en public) ;
  donnez-le en main propre ou par message privé au parent enregistré.
- Si une famille se plaint de ne **pas recevoir** son accès : vérifiez d'abord que son
  **email/mobile de parent** est correct (module *10-parents-tuteurs.md*), puis réinitialisez.
- Le compteur « Demandes en attente » doit revenir à **0** après traitement : s'il reste alto,
  formez les familles à utiliser le bouton « Mot de passe oublié » plutôt que de vous appeler.
- Cette page ne supprime **aucun** compte : elle change uniquement le mot de passe.
