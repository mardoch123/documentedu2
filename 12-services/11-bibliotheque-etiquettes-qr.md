---
id: 12-11-bibliotheque-etiquettes-qr
partie: 12
titre_partie: "Services annexes"
app: web
slug: 12-11-bibliotheque-etiquettes-qr
emoji: "🏷️"
titre: "Bibliothèque : imprimer les étiquettes QR des livres"
resume: "Chaque exemplaire reçoit une étiquette QR collée dans le livre."
audiences: [school_admin, staff]
---
# 🏷️ Bibliothèque : imprimer les étiquettes QR des livres

## 🎯 Rôle
Chaque **exemplaire** reçoit une **étiquette QR** collée dans le livre. Ce QR **identifie
l'exemplaire** et permet de **prêter / rendre en un scan** (voir *10*). Cette page **génère
et imprime** ces étiquettes, en **planche** à découper.

## ✅ Prérequis
1. Avoir des **livres/exemplaires** au catalogue (*09*).
2. Une **imprimante** (et des planches d'étiquettes autocollantes au format adapté).
3. Accès : menu **Library → Labels** (`library.labels.index`).

## 🟢 Générer le QR d'un exemplaire
1. Depuis la **fiche d'un livre** (*09*, `library.books.show`), sur l'**exemplaire** voulu,
   cliquez **« Générer le QR »** (`library.copies.generate-qr`).
2. Le QR de cet exemplaire est **créé** (il porte son identifiant unique).

## 🖨️ Imprimer une planche d'étiquettes (étape par étape)
1. Ouvrez **Labels** (`library.labels.index`).
2. **Sélectionnez** les exemplaires dont il faut imprimer les étiquettes (ou « tout »).
3. Lancez l'**impression** (`library.labels.print`) : une **planche PDF** d'étiquettes QR se
   génère.
4. **Imprimez** la planche sur les **étiquettes autocollantes**, puis **collez** chaque QR
   **dans son livre**.

## ✏️ Ré-imprimer une étiquette
- Étiquette **abîmée/perdue** : retournez dans **Labels**, **re-sélectionnez** l'exemplaire et
  **réimprimez** (`labels.print`) — le QR est **le même** (il dépend de l'exemplaire).

## 🔴 Retirer / ♻️ Restaurer
- Une étiquette ne se « supprime » pas dans le système : on **recolle** simplement une
  étiquette imprimée. Le **QR** reste **valide** tant que l'**exemplaire** existe.
- Exemplaire **retiré** (perdu / pilé) : il sort du service (*09*, statut) ; on peut **cesser
  de le scanner**. S'il **revient**, il redevient utilisable avec **son même QR**.

## ⚠️ Bon à savoir
- **Un QR par exemplaire** (pas par titre) : deux copies du même livre ont **deux QR
  différents**, pour suivre chaque prêt individuellement.
- **Scannez avec l'app** du personnel ou le scanner de la page prêts/retours (*10*) : prêt et
  retour deviennent **instantanés**.
- **Imprimez par lots** (une planche = plusieurs étiquettes) pour équiper un **rayon**
  d'un coup.
- **Protégez les QR** (film transparent) : ils vivent dans des livres manipulés par des
  enfants.
- Le même principe d'**étiquettes QR** existe pour le **mobilier** (*12*, inventaire physique).
