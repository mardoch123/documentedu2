---
id: 13-05-generateur-devoirs-ia
partie: 13
titre_partie: "Pédagogie quotidienne"
app: web
slug: 13-05-generateur-devoirs-ia
emoji: "🤖"
titre: "Générateur de devoirs par IA (payant, à crédits)"
resume: "Cet outil génère automatiquement des devoirs/exercices grâce à l'intelligence artificielle, à partir d'une classe et d'une leçon choisis."
audiences: [school_admin, teacher]
---
# 🤖 Générateur de devoirs par IA (payant, à crédits)

## 🎯 Rôle
Cet outil **génère automatiquement des devoirs/exercices** grâce à l'**intelligence
artificielle**, à partir d'une **classe** et d'une **leçon** choisis. Il produit un **sujet +
un corrigé**, exportables en **PDF**, et peut le **publier** comme devoir. ⚠️ C'est un
service **payant** fonctionnant par **crédits** (limite d'usage, rechargement).

## ✅ Prérequis
1. Être **Teacher** (ou Super Admin / avoir la permission « homework-generator-list »).
2. Avoir des **leçons** créées (*03*) pour nourrir la génération.
3. Disposer de **crédits** (le générateur en **consomme** à chaque usage).
4. Accès : menu **Homework Generator** (`homework-generator.index`).

## 🟢 Générer un devoir IA (étape par étape)
1. Ouvrez le **Générateur de devoirs**.
2. Choisissez la **classe/section** (`homework-generator.get-class-sections`) puis la
   **leçon** (`homework-generator.get-lessons`).
3. Lancez la **génération** (`homework-generator.generate`) : l'IA produit les **questions /
   exercices** et le **corrigé**.
4. **Relisez et ajustez** le résultat (`homework-generator.update`) avant diffusion : l'IA
   propose, **l'enseignant valide**.

## 🚀 Publier et exporter
- **Publier** le devoir généré aux élèves (`homework-generator.publish/{homework}`).
- **Exporter le sujet en PDF** (`homework-generator.export-pdf/{homework}`).
- **Exporter le corrigé** (`homework-generator.export-answer-key/{homework}`) — à garder pour
  l'enseignant.

## 💳 Crédits & paiement
1. **Vérifier la limite/les crédits** disponibles (`homework-generator.check-limit`) et
   l'**usage** (`homework-generator.usage-stats`).
2. Si les crédits manquent : **recharger / payer** (`homework-generator.process-payment`,
   retour via `payment-callback`) pour **racheter des crédits** de génération.

## ✏️ Modifier / 🔴 Supprimer un devoir généré
- **Modifier** avant publication : `homework-generator.update`.
- **Supprimer** un devoir généré (`homework-generator.destroy/{homework}`), puis
  **régénérer** si besoin.

## ♻️ Restaurer
- ⚠️ **Pas de corbeille** : un devoir IA supprimé se **recrée** par une **nouvelle
  génération** (ce qui **re-consomme un crédit**). **Exportez en PDF** ce que vous voulez
  garder avant de supprimer.

## ⚠️ Bon à savoir
- **Chaque génération consomme des crédits** : vérifiez le solde (`check-limit`) avant de
  lancer de gros volumes.
- **Toujours relire** la production de l'IA (erreurs possibles) : c'est une **aide**, pas un
  substitut à votre jugement pédagogique.
- **Corrigé séparé** : exportez le **corrigé** à part, **ne le diffusez pas** aux élèves.
- **Les leçons enrichissent la qualité** : un bon contenu de leçon (*03*) donne de meilleurs
  devoirs.
- Lié aux **devoirs classiques** (*04*) : le devoir IA publié rejoint le suivi des remises.
