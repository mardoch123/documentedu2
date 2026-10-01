# Configuration de Whatsapp

## 📱 Guide d'Utilisation Officiel : Module WhatsApp pour les Écoles

> **Plateforme EduEasy** \
> _&#x47;uide complet, illustré pas à pas et simplifié pour les directions d'école, administrateurs et secrétariats._

***

### 📋 Table des Matières

1. Introduction & Pourquoi WhatsApp ?
2. Aperçu de l'Expérience Parent / Smartphone
3. Configuration Meta WhatsApp Cloud API (Pas à Pas)
4. Activation & Paramétrage dans votre Espace École
5. Tableau de Bord & Statistiques en Temps Réel
6. Modèles Automatiques Déclenchés par les Événements
7. Création de Modèles Personnalisés & Variables Dynamiques
8. Envois Groupés & Campagnes Ciblées
9. Messages Programmés & Récurrents
10. Carnet d'Adresses & Contacts Externes
11. Suivi des Envois, Journaux (Logs) & Statuts de Lecture
12. Règles Meta & Bonnes Pratiques Anti-Spam
13. Foire Aux Questions (FAQ) & Dépannage

***

### 1. Introduction & Pourquoi WhatsApp ?

La communication école-famille est la clé de voûte de la réussite des élèves et du recouvrement des frais scolaires.

* ⚡ **Taux d'ouverture exceptionnel (> 98%)** : 9 messages sur 10 sont lus dans les 3 minutes suivant leur réception.
* 🚀 **Zéro friction pour les parents** : Pas d'application supplémentaire complexe à installer, les notifications arrivent directement sur leur messagerie quotidienne.
* 🔒 **Sécurité officielle Meta** : Canal certifié, garantissant l'authenticité de l'école et évitant le blocage de vos lignes.

***

### 2. Aperçu de l'Expérience Parent / Smartphone

Dès qu'une action est effectuée dans le logiciel EduEasy (saisie d'absence, encaissement de scolarité, publication d'un bulletin), le parent reçoit instantanément une notification élégante et officielle avec le nom de l'école :

***

### 3. Configuration Meta WhatsApp Cloud API (Pas à Pas)

Pour envoyer des messages avec l'identité de votre établissement, vous devez connecter votre compte Meta Developers.

#### Les 4 paramètres obligatoires :

1. **Phone Number ID** (Identifiant unique du numéro d'envoi).
2. **WhatsApp Business Account ID (WABA ID)** (Identifiant du compte d'entreprise).
3. **Jeton d'accès permanent (Permanent Access Token)**.
4. **URL de Webhook & Jeton de vérification (Verify Token)** (pour recevoir les statuts _Délivré_ et _Lu_).

***

#### 🛠️ Guide pas à pas sur Meta for Developers :

**Étape 1 : Créer votre Application Meta**

1. Rendez-vous sur [developers.facebook.com](https://developers.facebook.com) et connectez-vous avec votre compte Facebook.
2. Cliquez sur **Mes applications** (en haut à droite) > **Créer une application**.
3. Sélectionnez le type : **Autre** > puis cliquez sur **Professionnel** (ou _Business_).
4. Saisissez le nom de l'application (ex : `EduEasy - GS Sainte Marie`) et sélectionnez votre compte Business Manager.

**Étape 2 : Activer le Produit WhatsApp**

1. Dans le tableau de bord de votre application, faites défiler jusqu'à la section **WhatsApp** et cliquez sur **Configurer**.
2. Dans le menu de gauche, rendez-vous dans **WhatsApp** > **Démarrage rapide / Configuration de l'API**.
3. Vous y trouverez vos identifiants :
   * **Identifiant du numéro de téléphone (Phone Number ID)**
   * **Identifiant du compte WhatsApp Business (WABA ID)**

**Étape 3 : Créer un Jeton d'accès Permanent (System User Token)**

> ⚠️ **Important** : Le jeton temporaire expire après 24h. Créez un jeton permanent pour un fonctionnement sans interruption :

1. Rendez-vous dans les [Paramètres d'entreprise Meta](https://business.facebook.com/settings).
2. Dans le menu latéral : **Utilisateurs** > **Utilisateurs système** > Cliquez sur **Ajouter**.
3. Nommez l'utilisateur (ex : `EduEasy System`) et donnez-lui le rôle **Administrateur**.
4. Cliquez sur **Ajouter des actifs** > Sélectionnez votre Application WhatsApp et activez **Contrôle total**.
5. Cliquez sur **Générer un nouveau jeton** :
   * Sélectionnez votre application.
   * Cochez impérativement les permissions :
     * `whatsapp_business_messaging`
     * `whatsapp_business_management`
6. Copiez et conservez ce jeton d'accès permanent.

**Étape 4 : Configurer le Webhook (Accusés de lecture en direct)**

1. Dans le portail Meta Developers > **WhatsApp** > **Configuration**.
2. Dans le cadre **Webhook**, cliquez sur **Modifier** :
   * **URL de rappel (Callback URL)** : Collez l'URL indiquée dans votre espace EduEasy (ex: `https://edueasy.net/api/whatsapp/webhook/code_ecole`).
   * **Jeton de vérification (Verify Token)** : Collez le token affiché dans vos paramètres EduEasy.
3. Cliquez sur **Vérifier et enregistrer**.
4. Cliquez sur **Gérer les champs** et cochez le champ **messages**.

***

### 4. Activation & Paramétrage dans votre Espace École

1. Connectez-vous à votre portail **Administrateur École**.
2. Dans le menu de navigation, cliquez sur **WhatsApp** (ou **Paramètres** > **WhatsApp**).
3. Remplissez le formulaire de configuration :
   * Cochez **Activer le service WhatsApp**.
   * Collez votre **Phone Number ID**.
   * Collez votre **Business Account ID**.
   * Collez votre **Jeton d'accès permanent**.
4. Cliquez sur **Enregistrer les paramètres**.
5. Cliquez sur le bouton vert **Tester la connexion** : une notification de test valide instantanément que vos identifiants sont corrects !

***

### 5. Tableau de Bord & Statistiques en Temps Réel

Le tableau de bord WhatsApp vous offre une vue panoramique sur votre communication :

#### Indicateurs clés (KPIs) :

* 📤 **Envoyés Aujourd'hui** : Nombre de messages délivrés dans la journée.
* 📅 **Messages ce mois** : Consommation mensuelle cumulée.
* ❌ **Échecs** : Nombre de tentatives échouées (avec lien direct vers le motif).
* 💳 **Limite restante** : Solde ou quota de messages disponibles sur votre forfait.
* 📈 **Graphique d'activité** : Courbe des envois sur les 7 derniers jours pour observer les pics de communication (ex: périodes d'examens ou de fin de mois).

***

### 6. Modèles Automatiques Déclenchés par les Événements

Le système envoie automatiquement des messages ciblés lors des actions administratives et pédagogiques du quotidien :

| Événement                   | Déclencheur dans EduEasy                   | Destinataire   | Variables automatiques disponibles                         |
| --------------------------- | ------------------------------------------ | -------------- | ---------------------------------------------------------- |
| **Admission / Inscription** | Validation de la fiche d'un nouvel élève   | Parent         | `{student_name}`, `{class_name}`, `{school_name}`          |
| **Absence**                 | Enseignant ou CPE marquant un élève absent | Parent         | `{student_name}`, `{date}`, `{school_name}`                |
| **Retard**                  | Pointage d'un retard à l'entrée            | Parent         | `{student_name}`, `{time}`, `{date}`                       |
| **Paiement Reçu**           | Enregistrement d'un encaissement en caisse | Parent         | `{student_name}`, `{amount}`, `{receipt_no}`, `{fee_name}` |
| **Rappel d'Échéance**       | Date d'exigibilité de tranche de scolarité | Parent         | `{student_name}`, `{amount}`, `{due_date}`, `{fee_name}`   |
| **Bulletin de Notes**       | Clôture et publication des bulletins       | Parent         | `{student_name}`, `{session_year}`, `{term}`, `{url}`      |
| **Nouveau Devoir**          | Devoir publié sur l'espace élève           | Parent / Élève | `{student_name}`, `{subject}`, `{due_date}`                |
| **Conseil de Discipline**   | Convocation disciplinaire émise            | Parent         | `{student_name}`, `{meeting_date}`, `{reason}`             |

> 💡 **Personnalisation** : Vous pouvez activer ou désactiver chaque événement individuellement et adapter le texte selon les formules de politesse de votre établissement.

***

### 7. Création de Modèles Personnalisés & Variables Dynamiques

Pour vos annonces ponctuelles (fêtes de l'école, réunions de parents, fermetures exceptionnelles), vous pouvez créer vos propres modèles dans l'onglet **Modèles Personnalisés**.

#### Les Variables Dynamiques Reconnues :

* `{student_name}` : Prénom et nom de l'élève.
* `{parent_name}` : Prénom et nom du parent / tuteur.
* `{class_name}` : Nom de la classe (ex: `Terminale S`, `6ème B`).
* `{school_name}` : Nom officiel de votre école.
* `{amount}` : Montant avec devise (ex: `120 000 FCFA` ou `1 500 000 GNF`).
* `{due_date}` : Date d'échéance.
* `{date}` : Date courante.

#### Exemple de modèle de convocation :

```
Chers parents de {student_name},

La direction de {school_name} vous convie à l'assemblée générale de début d'année pour la classe de {class_name}, qui se tiendra ce samedi à 09h30 dans la salle polyvalente.

Votre présence est indispensable pour la validation du calendrier des examens.

Bien cordialement,
Le Secrétariat
```

***

### 8. Envois Groupés & Campagnes Ciblées

Dans l'onglet **Envoi Groupé** :

1. **Choisissez votre cible** :
   * **Par Rôle** : Tous les Parents, Tous les Enseignants, Tous les Élèves, ou Tout le Personnel.
   * **Par Classe & Section** : Ciblez une ou plusieurs classes spécifiques (ex : uniquement les classes de 3ème et Terminale).
   * **Import de liste CSV / Excel** : Téléversez un fichier de numéros pour des campagnes externes (invitations de partenaires, anciens élèves).
2. **Sélectionnez le modèle ou rédigez le message**.
3. **Ajoutez un média si nécessaire** (Image d'affiche, document PDF du règlement intérieur, etc.).
4. Cliquez sur **Envoyer** : les messages sont distribués en tâche de fond à grande vitesse sans ralentir votre navigation.

***

### 9. Messages Programmés & Récurrents

Anticipez votre communication grâce au planificateur de tâches :

1. Rendez-vous dans **Messages Programmés** > **Créer une programmation**.
2. Définissez la **date et l'heure précise** d'envoi.
3. Choisissez le type de récurrence :
   * **Ponctuel** : Envoyé une seule fois à la date fixée.
   * **Hebdomadaire** : Tous les vendredis après-midi par exemple.
   * **Mensuel** : Le 25 de chaque mois pour le rappel des mensualités de scolarité.
4. Le système déclenche les envois automatiquement sans intervention humaine.

***

### 10. Carnet d'Adresses & Contacts Externes

L'onglet **Contacts** centralise les numéros hors-élèves :

* Membres du conseil d'administration.
* Prestataires et transporteurs scolaires.
* Inspecteurs et partenaires académiques.
* Regroupement par étiquettes et catégories pour des envois en 1 clic.

***

### 11. Suivi des Envois, Journaux (Logs) & Statuts de Lecture

Chaque message envoyé dispose d'un suivi détaillé dans l'onglet **Journaux (Logs)** :

```
[25/08/2026 10:15] Lucas Dubois (Parent: M. Dubois) → Reçu de Paiement • Statut: Lu 🟣
[25/08/2026 09:32] Sarah Camara (Parent: Mme Camara) → Alerte Absence • Statut: Délivré 🔵
[25/08/2026 08:45] Jean Touré (Parent: M. Touré) → Rappel Frais • Statut: Échoué 🔴 [Numéro Invalide] ↺ Réessayer
```

#### Signification des Statuts :

* 🟡 **En attente (Pending)** : Message en cours d'expédition par la file de traitement.
* 🟢 **Envoyé (Sent)** : Transmis aux serveurs Meta WhatsApp.
* 🔵 **Délivré (Delivered)** : Reçu sur le smartphone du parent (2 coches grises).
* 🟣 **Lu (Read)** : Message ouvert et lu par le destinataire (2 coches bleues).
* 🔴 **Échoué (Failed)** : Échec d'envoi. Cliquez sur l'icône pour voir la cause exacte et réexpédier après correction.

***

### 12. Règles Meta & Bonnes Pratiques Anti-Spam

Pour préserver la réputation de votre numéro et assurer 100% de délivrabilité :

1. **Format International Obligatoire des Numéros** :
   * Les numéros de téléphone doivent obligatoirement être enregistrés avec leur indicatif pays complet (sans `+` ni `00`) :
     * 🇬🇳 **Guinée** : `224620000000`
     * 🇸🇳 **Sénégal** : `221770000000`
     * 🇨🇮 **Côte d'Ivoire** : `225070000000`
     * 🇧🇯 **Bénin** : `22997000000`
     * 🇹🇬 **Togo** : `22890000000`
     * 🇨🇲 **Cameroun** : `23760000000`
     * 🇲🇱 **Mali** : `22370000000`
     * 🇧🇫 **Burkina Faso** : `22670000000`
2. **Fenêtre de 24 Heures Meta** :
   * Lorsqu'un parent vous envoie un message, vous disposez d'une fenêtre de 24h pour échanger librement.
   * Les notifications automatiques initiées par l'école utilisent des modèles structurés et approuvés pour garantir leur passage en toutes circonstances.
3. **Heures d'envoi respectueuses** :
   * Privilégiez les envois entre 07h30 et 19h30 pour ne pas déranger les familles hors des heures scolaires.

***

### 13. Foire Aux Questions (FAQ) & Dépannage

**Q1 : Que faire si le test de connexion indique "Authentication failed" ?**

**R :** Vérifiez que votre jeton d'accès n'a pas expiré et qu'il possède bien les autorisations `whatsapp_business_messaging` et `whatsapp_business_management`. Utilisez impérativement un jeton d'utilisateur système permanent.

**Q2 : Pourquoi un parent ne reçoit-il pas les messages ?**

**R :** Vérifiez dans l'onglet **Journaux (Logs)** :

1. Le numéro contient-il bien l'indicatif international ?
2. Le parent a-t-il installé WhatsApp sur ce numéro ?
3. Si le message est marqué _Échoué_, cliquez sur le bouton **Détails de l'erreur** pour afficher la réponse exacte de Meta.

**Q3 : Les enseignants peuvent-ils envoyer des messages WhatsApp depuis leur compte ?**

**R :** Oui, si l'administrateur de l'école leur a accordé la permission de communication WhatsApp dans la gestion des rôles et autorisations.

***

_Documentation officielle EduEasy — Version 2026. Tous droits réservés._
