# F02 — Instructions officielles de réalisation et de remise

## 1 — Cloner votre fork et préparer votre branche EN LOCAL

1. Ouvrez [le dépôt officiel](https://github.com/terra1313/13Layers_Bootcamp_F), puis cliquez sur **Fork**. Choisissez votre compte GitHub personnel.
2. **Clonez votre fork** sur votre ordinateur (remplacez `VOTRE_PSEUDO` par votre identifiant GitHub).
3. **Entrez dans `formations/F02-Linux` avant de créer une branche** :

```bash
git clone https://github.com/VOTRE_PSEUDO/13Layers_Bootcamp_F.git
cd 13Layers_Bootcamp_F
git switch main
git pull origin main
cd formations/F02-Linux
git switch -c Bootcamp_F02__prenom_nom
mkdir -p devoirs/prenom-nom/preuves devoirs/prenom-nom/scripts
```

Remplacez `prenom-nom` et `prenom_nom` par votre nom, en minuscules sans espace ni accent. Exemple : `Bootcamp_F02__jean_doe`.

**Important :** ne créez pas vos fichiers dans `Bootcamp-F01`, dans `formations/F01-Git-GitHub`, ni à la racine du dépôt. Une branche Git reste globale au dépôt même si on l'a créée depuis le dossier F02.

## 2 — Suivre le cours officiel

Suivez le cours OpenClassrooms **[Initiez-vous à Linux](https://openclassrooms.com/fr/courses/7170491-initiez-vous-a-linux)** **jusqu'au bout**.

- Terminez tous les chapitres et validez **chacun des 3 quiz**.
- Faites **une ou plusieurs captures d'écran** montrant clairement **les trois quiz au vert et la formation terminée**.
- Si une seule capture ne montre pas tout, fournissez plusieurs images lisibles.
- Enregistrez vos preuves sous `devoirs/prenom-nom/preuves/`, par exemple `openclassrooms_formation_terminee.png` et `openclassrooms_quiz_valides.png`.
- Masquez les informations personnelles sans intérêt pour la preuve.

## 3 — Questions et travaux pratiques

- Répondez aux [10 questions](01_CATALOGUE_QUESTIONS.md) dans votre `devoirs/prenom-nom/REPONSES_F02.md`.
- Réalisez **tous les exercices** de [02_TRAVAUX_PRATIQUES.md](02_TRAVAUX_PRATIQUES.md), et inscrivez **les réponses, commandes, sorties et commentaires** dans `devoirs/prenom-nom/RAPPORT_TP.md`.
- Fournissez les scripts demandés dans `devoirs/prenom-nom/scripts/`.
- Complétez la fiche `FICHE_SUIVI.md` et répondez notamment à **« Comment avez-vous trouvé cette formation ? »**.

**Organisation obligatoire dans votre fork :**

```text
formations/F02-Linux/
├── README.md
├── 01_CATALOGUE_QUESTIONS.md
├── 02_TRAVAUX_PRATIQUES.md
├── 03_CONSIGNES_REMISE.md
├── templates/
│   ├── REPONSES_F02.md
│   ├── RAPPORT_TP.md
│   └── FICHE_SUIVI_F02.md
└── devoirs/
    └── prenom-nom/
        ├── REPONSES_F02.md
        ├── RAPPORT_TP.md
        ├── FICHE_SUIVI.md
        ├── scripts/
        │   ├── demo.sh
        │   └── system_info.sh
        └── preuves/
            ├── openclassrooms_formation_terminee.png
            └── openclassrooms_quiz_valides.png
```

Depuis `formations/F02-Linux`, copiez les modèles dans le dossier étudiant :

```bash
cp templates/REPONSES_F02.md devoirs/prenom-nom/REPONSES_F02.md
cp templates/RAPPORT_TP.md devoirs/prenom-nom/RAPPORT_TP.md
cp templates/FICHE_SUIVI_F02.md devoirs/prenom-nom/FICHE_SUIVI.md
```

## 4 — Tester, pousser et ouvrir une Pull Request

```bash
# Exécuter depuis formations/F02-Linux
bash -n devoirs/prenom-nom/scripts/*.sh
git status
git add devoirs/prenom-nom/
git commit -m "feat(F02): exercices Linux prenom nom"
git push -u origin Bootcamp_F02__prenom_nom
```

Dans GitHub : ouvrez la PR **de votre fork, branche `Bootcamp_F02__prenom_nom`, vers `terra1313/13Layers_Bootcamp_F:main`**. Titre : **`[F02] Prénom Nom — Linux`**. Remplissez le template de PR.

**Le formateur évalue les devoirs par PR ; ne fusionnez pas la PR dans `main` !** Une PR acceptée peut être fermée sans fusion pour conserver un dépôt pédagogique propre.

## 5 — Liste de contrôle

- [ ] Je suis entré dans le dossier F02 et j'ai créé la branche avant de modifier les fichiers.
- [ ] J'ai terminé « Initiez-vous à Linux ».
- [ ] Tous les quiz OpenClassrooms apparaissent au vert sur mes captures.
- [ ] La capture prouve la fin de la formation.
- [ ] J'ai répondu aux 10 questions et aux 6 TP.
- [ ] Mes scripts fonctionnent et je les ai testés.
- [ ] J'ai rempli ma fiche de suivi et donné mon avis.
- [ ] Je n'ai ajouté aucun secret ni donnée privée.
- [ ] J'ai poussé sur mon fork et ouvert ma PR.
