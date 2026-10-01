---
id: 17-04-scan-qr-presence
partie: 17
titre_partie: "Application EduStaff"
app: edustaff
slug: 17-04-scan-qr-presence
emoji: "📷"
titre: "scanner le QR de présence (arrivée/départ) et suivre l'historique"
resume: "Le scan du QR-code affiché à l'école remplace la feuille d'émargement : chacun pointe son arrivée et son départ en 2 secondes, avec l'heure et la position enregistrées automatiquement."
audiences: [teacher, staff, school_admin]
---
# 📷 17.4 — EduStaff : scanner le QR de présence (arrivée/départ) et suivre l'historique

## 🎯 Rôle
Le **scan du QR-code affiché à l'école** remplace la feuille d'émargement : chacun
pointe son **arrivée** et son **départ** en 2 secondes, avec l'heure et la position
enregistrées automatiquement. La direction consulte l'historique et traite les
justifications.

## ✅ Prérequis
1. Être connecté à EduStaff (page 17.1).
2. **Autoriser la caméra** quand le téléphone la demande (première fois).
3. **Activer le GPS (localisation)** : ⚠️ sans position, le scan est refusé — message
   « La géolocalisation est requise pour scanner. Activez le GPS et réessayez. »
4. Que l'école affiche son **QR-code de présence** (accueil, bureau, salle des profs) —
   généré sur le web EduEasy (PARTIE 08).

## 🟢 Pointer son arrivée ou son départ (étape par étape)
1. Accueil → bouton **« + »** → famille **Outils** → **« Scanner QR présence »**
   (ou la tuile dédiée si votre accueil la montre).
2. Laissez l'écran démarrer la caméra (« Démarrage de la caméra… »).
3. Cadrez le QR-code de l'école dans le **rectangle** de l'écran.
   En zone sombre, touchez l'icône **flash** pour éclairer.
4. Le téléphone vibre : l'écran confirme les données lues et **choisit tout seul le
   type d'action** — « Arrivée » avant midi, « Départ » après midi.
5. Vérifiez l'information puis appuyez sur **Confirmer**.
6. Message de succès : votre présence est enregistrée à l'**heure exacte**, avec la
   position « École » (latitude/longitude capturées au moment de la confirmation).
7. Le scanner redémarre automatiquement pour la personne suivante.

## 🟢 Consulter l'historique QR
1. Écran du scanner → icône **Historique** (ou menu « Historique QR »).
2. La liste montre vos pointages : **Type** (Étudiant/Staff), **Action** (Arrivée ou
   Départ), **Heure**, **Lieu**.
3. Touchez **« Filtrer »** (icône entonnoir) pour restreindre par période ou par type.
4. Message « Aucun historique QR trouvé » : vous n'avez pas encore pointé, ou le filtre
   est trop strict.

## 🟢 Direction : traiter les justifications (écran « Demandes d'explication (QR) »)
1. Accueil → bouton **« + »** → famille **Validations & Suivi** →
   **« Demandes d'explication (QR) »**.
2. En haut, trois **indicateurs** : total des demandes, **en attente**, traitées.
3. Ouvrez une demande **En attente** : l'enseignant y a indiqué l'heure réelle de départ
   et le motif (oubli de scan, connexion, batterie…).
4. Décidez : touchez **« Enregistrer la régularisation »** pour valider — les heures de
   la journée sont **corrigées automatiquement** ; ou refusez en précisant pourquoi.
5. Le demandeur voit le résultat dans son onglet « Traitées » (page 17.3).

## ✏️ Modifier
- Une présence QR mal enregistrée (mauvaise heure, double scan) **ne se corrige pas
  dans l'app** : la direction rectifie sur le web (PARTIE 08) ou valide une
  justification (étapes ci-dessus).
- Le **type d'action** (arrivée/départ) est calculé selon l'heure : impossible de le
  forcer manuellement dans l'app.

## 🔴 Supprimer
- On ne **supprime pas** un pointage depuis l'application : c'est un journal de
  présence, il doit rester fiable.
- La direction peut effacer/corriger une ligne sur le web EduEasy (PARTIE 08), avec
  traçabilité.

## ♻️ Restaurer
- **QR refusé « invalide »** : le code affiché n'est pas celui de l'école (capture d'un
  autre écran, QR périmé) — faites scanner le QR original affiché à l'école.
- **Caméra refusée par erreur** : Réglages du téléphone → Applications → EduStaff →
  Autorisations → réactivez **Caméra** et **Localisation**.
- **Pointage perdu** (application fermée avant confirmation) : recommencez le scan,
  l'heure réelle du scan est enregistrée, pas la précédente.
- Historique vide alors que vous pointez d'habitude : vérifiez le filtre, puis
  déconnectez-reconnectez pour re-synchroniser.

## ⚠️ Bon à savoir
- Le scan exige d'**être physiquement à l'école** (position GPS) : impossible de pointer
  depuis chez soi — c'est voulu.
- Avant midi = **arrivée**, après midi = **départ** : si vous scannez à 11h59 puis
  12h01, vous obtenez les deux bonnes actions.
- En cas d'oubli de scan de **départ**, justifiez-le le jour même (page 17.3) : la
  régularisation automatique corrige vos heures.
- **Panne de téléphone** ou batterie à plat au moment du départ : motif « Batterie de
  téléphone déchargée » dans la justification.
- Les enseignants ne voient dans l'historique que **leurs** pointages ; la direction
  voit tous les pointages (personnel et élèves selon les modules activés).
