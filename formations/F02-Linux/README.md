# F02 — Linux & ligne de commande

**13Layers Academy · Roadmap DevOps · Module F02**

## Étape 1 — Formation OpenClassrooms obligatoire

Suivez intégralement le cours **[Initiez-vous à Linux — OpenClassrooms](https://openclassrooms.com/fr/courses/7170491-initiez-vous-a-linux)**.

**Preuve obligatoire :** une ou plusieurs captures d'écran démontrant que **tous les quiz du cours sont validés (au vert)** et que **le cours est terminé**. Les quiz du cours concernent les premiers pas sur Linux, Linux comme poste de travail et Linux dans l'activité professionnelle. Masquez toute donnée privée inutile.

## Étape 2 — Réponses et exercices

1. Répondez aux [10 questions du catalogue](01_CATALOGUE_QUESTIONS.md).
2. Réalisez les [6 travaux pratiques Linux](02_TRAVAUX_PRATIQUES.md) en local (Ubuntu, VM ou WSL).
3. Pour **chaque question et chaque TP**, indiquez les commandes exécutées, résultats et explications lorsque cela est pertinent.
4. Complétez la [fiche de suivi](templates/FICHE_SUIVI_F02.md) et le [modèle de réponses](templates/REPONSES_F02.md).

## Étape 3 — Travail local et remise GitHub

Depuis **votre fork cloné en local**, entrez d'abord dans le dossier de la formation :

```bash
cd 13Layers_Bootcamp_F/formations/F02-Linux
git switch -c Bootcamp_F02__prenom_nom
mkdir -p devoirs/prenom-nom/preuves devoirs/prenom-nom/scripts
```

**Créez la branche avant toute modification.** Une branche Git concerne le dépôt entier ; vos fichiers doivent être modifiés **uniquement dans `formations/F02-Linux/devoirs/prenom-nom/`** de votre fork.

Suivez pas à pas les [consignes officielles de remise](03_CONSIGNES_REMISE.md), puis ouvrez une Pull Request vers le dépôt officiel.

## Évaluation /100
| Critère | Points |
|---|---:|
| 10 questions théoriques | 40 |
| TP1 à TP5 | 35 |
| TP6 — script Bash | 10 |
| Qualité du compte rendu | 5 |
| Capture de formation terminée + bilan personnel | 10 |
| **Total** | **100** |

**Sécurité :** pas de commande destructrice ou de secret dans les rendus.
