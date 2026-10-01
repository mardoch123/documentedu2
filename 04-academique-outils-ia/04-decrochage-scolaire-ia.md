---
id: 04-04-decrochage-scolaire-ia
partie: 4
titre_partie: "Académique : Outils IA"
app: web
slug: 04-04-decrochage-scolaire-ia
emoji: "📘"
titre: "Décrochage Scolaire (détection IA)"
resume: "Repérer avant qu'il ne soit trop tard les élèves qui risquent de quitter l'école : l'IA croise les absences, les notes en baisse, les impayés et les signalements, puis classe cha"
audiences: [school_admin]
---
# Décrochage Scolaire (détection IA)

## 🎯 Rôle
Repérer **avant qu'il ne soit trop tard** les élèves qui risquent de quitter l'école :
l'IA croise les absences, les notes en baisse, les impayés et les signalements, puis
classe chaque élève à risque (faible / moyen / élevé) avec les motifs de l'alerte.

## ✅ Prérequis
- Que l'école **saisit déjà** des présences et des notes (sinon l'IA n'a rien à analyser).
- Accès : menu **Académique → Décrochage Scolaire (IA)**.

## 🟢 Consulter et traiter les alertes
1. Ouvrez **Décrochage Scolaire (IA)**.
2. Le tableau liste les élèves suivis avec :
   - un **score de risque** (0 à 100) et un niveau coloré (vert / orange / rouge) ;
   - les **motifs** : ex. « 6 absences en 3 semaines », « moyenne en baisse de 3 points »,
     « 2 mois de frais impayés ».
3. Cliquez sur un élève pour ouvrir son **profil de risque** (historique des signaux).
4. Choisissez une **action de rétention** :
   - **Contacter le parent** → bouton WhatsApp/SMS/Email qui pré-remplit un message ;
   - **Passer en conseil de discipline/engagement** → crée le brouillon correspondant ;
   - **Marquer « traité »** avec une note interne pour ne plus voir l'alerte.
5. Periodiquement, filtrez sur « Non traités » pour votre revue de semaine.

## ✏️ Ajuster l'analyse
- Un élève signalé à tort (ex. absences justifiées) : ouvrez sa fiche absence et
  **justifiez les pointages** — le score recalcule tout seul.
- Les seuils de déclenchement peuvent être réglés depuis la page (curseurs ou
  paramètres du module, selon version) : plus sensibles = plus d'alertes.

## 🔴 Supprimer une alerte
Les alertes ne se « suppriment » pas : elles se **clôturent**
(bouton **Traité / Ignorer**). Une alerte ignorée peut resurgir si les signaux
repassent au rouge — c'est voulu.

## ♻️ Réouvrir une alerte traitée
1. Filtre **« Traitées »** de la liste.
2. Sur la ligne, bouton **Rouvrir / Réinclure** → l'élève repart dans la liste active.

## ⚠️ Bon à savoir
- Cette donnée est **sensible** : ne discutez jamais d'un « élève à risque » devant lui
  ou devant d'autres élèves ; la liste est réservée à la direction et aux conseillers.
- Une absence mal pointée par un prof fausse tout : la qualité de cet outil dépend de
  la discipline de saisie des présences (voir 08-presences).
- L'IA ne prend **aucune décision** : elle propose, un adulte décide.
