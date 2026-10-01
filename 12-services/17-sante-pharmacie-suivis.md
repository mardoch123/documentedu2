---
id: 12-17-sante-pharmacie-suivis
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-17-sante-pharmacie-suivis
emoji: "💊"
titre: "Santé : pharmacie (stock médicaments), suivis et statistiques"
resume: "Cette page ferme le cycle santé : la pharmacie gère le stock de médicaments de l'infirmerie (entrées, sorties, délivrance sur ordonnance), les suivis médicaux (recontrôles d'un é"
audiences: [school_admin, staff]
---
# 💊 Santé : pharmacie (stock médicaments), suivis et statistiques

## 🎯 Rôle
Cette page ferme le cycle santé : la **pharmacie** gère le **stock de médicaments** de
l'infirmerie (entrées, sorties, **délivrance** sur ordonnance), les **suivis médicaux**
(recontrôles d'un élève après une consultation) et les **statistiques** globales du service
(maladies fréquentes, consommations, absences médicales).

## ✅ Prérequis
1. Avoir des **ordonnances/consultations** (*15*, *16*) et un **stock** initialisé.
2. Option « Health / Medical » + permissions pharmacie/santé.
3. Accès : menu **Health → Pharmacie** (`health.pharmacy.index`), **Suivis**
   (`health.followups.index`), **Statistiques** (`health.statistics`).

## 💊 Gérer le stock de médicaments
1. **Ajouter un médicament** au stock (`health.pharmacy.store`) : **nom**, **dosage**,
   **forme**, **quantité**, **date de péremption**, **prix** éventuel.
2. **Entrées / sorties de stock** :
   - **Réapprovisionner** : `health.pharmacy.add-stock/{id}` (on **ajoute** des unités) ;
   - **Retirer** (perte, péremption) : `health.pharmacy.remove-stock/{id}`.
3. **Mouvements d'un médicament** (`health.pharmacy.movements/{id}`) : **journal** de tout ce
   qui est **rentré/sorti** (traçabilité du stock).
4. **Liste des médicaments** (`health.pharmacy.medicines-list`) : état complet du stock.

## 🚚 Délivrer un médicament (sur ordonnance)
1. Ouvrez **Dispensing / Délivrer** (`health.pharmacy.dispensing`).
2. Retrouvez l'**ordonnance** à servir ; **validez la délivrance**
   (`health.pharmacy.dispense/{prescription}`) : le **stock du médicament diminue** d'autant.
3. La **délivrance** est **liée à l'ordonnance et à l'élève** (traçabilité).

## 📅 Suivis médicaux (contrôles)
1. Ouvrez **Suivis** (`health.followups.index`).
2. Après une consultation nécessitant un **recontrôle**, ajoutez un **suivi rapide**
   (`health.followups.quick/{consultation}`) : date du contrôle, observation, évolution.
3. Les suivis apparaissent dans le **dossier** de l'élève (*15*).

## 📊 Statistiques du service santé
- `health.statistics` : **indicateurs** (consultations, pathologies fréquentes, médicaments
  consommés, élèves suivis) — pour le **reporting** et la **médecine préventive**.

## ✏️ / 🔴 / ♻️ Ajuster, retirer, restaurer
- Le **stock** s'**ajuste par ajout / retrait** (`add-stock` / `remove-stock`) plutôt que par
  suppression : chaque mouvement est **journalisé** (`movements`).
- ⚠️ **Pas de corbeille** : un médicament **périme** (sortie de stock) et se **recrège** par
  une **nouvelle entrée** ; une **délivrance** erronée se compense par un **ajustement de
  stock** inverse. L'**historique reste intègre** (exigence pharmaceutique).

## ⚠️ Bon à savoir
- **Dates de péremption** : surveillez-les (tri par péremption) et **sortez** les produits
  périmés (`remove-stock`).
- **Seuil bas** : réapprovisionnez **avant** la rupture (`add-stock`) pour ne pas refuser une
  délivrance.
- **Délivrance = ordonnance** : ne dispensez que sur **ordonnance enregistrée** (*16*), pour
  la **traçabilité** élève ↔ médicament.
- Les **statistiques** aident à commander le **bon stock** (consommation réelle) et à repérer
  les **problèmes de santé récurrents** dans l'école.
- Accès **restreint** : la pharmacie et les suivis touchent à des **données médicales
  confidentielles**.
