---
id: 08-07-notifications
partie: 8
titre_partie: "Présences & communication"
app: web
slug: 08-07-notifications
emoji: "🔔"
titre: "Envoyer une notification (message par rôle)"
resume: "La notification est un message diffusé à un ou plusieurs rôles de l'école (ex."
audiences: [school_admin, teacher, staff]
---
# 🔔 Envoyer une notification (message par rôle)

## 🎯 Rôle
La **notification** est un message **diffusé à un ou plusieurs rôles** de l'école
(ex. tous les Parents, tous les Enseignants, tout le Personnel, tous les Élèves…),
éventuellement avec une **image**. Elle atterrit dans la **cloche de notification** et le
**Journal d'activités** des destinataires. C'est le canal tout indiqué pour une alerte
globale : fermeture exceptionnelle, rappel de réunion, consigne générale.

> Différence à retenir :
> - **Notification** = ciblée par **rôles** (catégories d'utilisateurs).
> - **Annonce** = ciblée par **classes/sections**, avec pièces jointes
>   (voir *06-annonces.md*).

## ✅ Prérequis
1. Permission « **notification-create** » (direction / Super Admin).
2. Avoir défini les **rôles** existants (Parents, Enseignants, Personnel, Élèves…).
3. Accès : menu latéral **Communication → Notifications**.

## 🟢 Créer et envoyer une notification (étape par étape)
1. Ouvrez le menu **Notifications**. Le bloc **« Créer une notification »** est en haut.
2. Choisissez le **type de destinataires** (boutons radio ★) :
   - **« Roles »** : envoyer à des rôles classiques (Parents, Profs, Personnel, Élèves) ;
   - **« Over Due Fees »** : envoyer uniquement aux **familles en retard de frais**
     (relance de paiement).
3. Sélectionnez le ou les **rôles** concernés dans la liste déroulante multi-choix
   **« roles »** ★ (maintenez Ctrl / cliquez plusieurs éléments pour en choisir plusieurs).
4. Renseignez :
   - **« title »** ★ — objet de la notification ;
   - **« message »** ★ — le corps du message ;
   - **Image** (facultatif) — une illustration jointe au message.
5. Cliquez sur le bouton d'envoi / **submit**.
6. La notification est **immédiatement visible** par tous les destinataires du rôle choisi
   (cloche en haut + historique).

## 📋 Consulter l'historique des notifications
- Le tableau dresse l'**historique des notifications envoyées** aux familles et au personnel :
  titre, message, destinataires, date.
- La **recherche**, les **colonnes** et le **rafraîchissement** aident à retrouver un envoi.

## ✏️ Modifier une notification
1. Sur la ligne concernée, cliquez l'**icône Modifier**.
2. La fenêtre d'édition reprend **titre**, **message**, **rôles** et **image**.
3. Corrigez puis **enregistrez**. (Modifier un envoi déjà lu par certains ne « rappelle »
   pas le message : l'action la plus sûre reste d'envoyer une **nouvelle** notification.)

## 🔴 Supprimer une notification
1. Sur la ligne, cliquez l'**icône Supprimer**, puis **confirmez**.
2. ⚠️ La suppression est **définitive** : les notifications **ne passent pas dans une
   corbeille restaurable** (contrairement aux annonces).

## ♻️ Restaurer une notification supprimée
Il n'existe **aucune restauration** pour les notifications une fois supprimées.
- **Recours** : **recréez** la notification à l'identique (titre + message + rôles) et
  renvoyez-la. C'est court, mais le message doit être resaisi.
- Gardez une **copie de vos messages importants** (dans un fichier) pour pouvoir les
  recoller rapidement en cas de suppression accidentelle.

## ⚠️ Bon à savoir
- Le type **« Over Due Fees »** est une **relance de paiement** ciblée : utilisez-le plutôt
  qu'un message général pour rappeler les impayés, il ne touchera que les familles concernées.
- Une notification **part à tous les rôles sélectionnés d'un coup** : vérifiez bien la liste
  avant d'envoyer (impossible de « retirer » un destinataire après coup).
- **Pas de corbeille** ici : réfléchissez avant de supprimer. Si vous voulez juste masquer
  une information, mieux vaut ne pas l'envoyer plutôt que de l'envoyer puis la supprimer.
- Pour du **SMS ou WhatsApp effectif** aux familles, il faut paramétrer les passerelles de
  messagerie de l'école (module Communication / SMS) ; la notification interne, elle, passe
  par l'application.
