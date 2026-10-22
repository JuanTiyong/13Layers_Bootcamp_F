# Règles de contribution — 13Layers Academy

## Organisation permanente

- Le dépôt officiel : `terra1313/13Layers_Bootcamp_F`.
- Les formations : `formations/F01-Git-GitHub/`, `formations/F02-Linux/`, puis `formations/F03-.../`, etc.
- **Chaque étudiant crée son propre fork.** Pas de commit direct sur `main`.
- **Chaque étudiant rend son devoir dans le dossier du module étudié** : `formations/FXX-Nom/devoirs/prenom-nom/`, dans **son fork**.
- Le devoir se soumet par PR vers `terra1313/13Layers_Bootcamp_F:main` ; le formateur évalue, approuve ou commente, puis peut fermer **sans fusion** pour ne pas polluer `main`.
- Les dossiers de devoirs F01 déjà publiés ont été rangés dans F01 ; ne les renommez pas ou ne les modifiez pas.

## Démarrage local (exemple F02)

```bash
git clone https://github.com/VOTRE_PSEUDO/13Layers_Bootcamp_F.git
cd 13Layers_Bootcamp_F
git switch main
git pull origin main
cd formations/F02-Linux
git switch -c Bootcamp_F02__prenom_nom
mkdir -p devoirs/prenom-nom/preuves devoirs/prenom-nom/scripts
```

**Ordre obligatoire :** cloner le fork → entrer dans le dossier F02 → créer la branche **avant** de modifier les fichiers → réaliser le travail. Une branche Git concerne le **dépôt entier**, même lorsqu'elle est créée depuis le sous-dossier F02 : veillez donc à ne modifier que votre dossier personnel dans ce module.

Copiez les modèles depuis `formations/F02-Linux/templates/`. Complétez-les, ajoutez vos scripts et une capture OpenClassrooms attestant la **fin du cours et les trois quiz au vert**, sans divulguer de données sensibles.

```bash
# Toujours depuis formations/F02-Linux, après les exercices :
git status
git add devoirs/prenom-nom/
git commit -m "feat(F02): devoir Linux prenom nom"
git push -u origin Bootcamp_F02__prenom_nom
```

Ouvrez la PR **depuis le fork**, avec le titre `[F02] Prénom Nom — Linux`. Le template PR doit être rempli.

## Règles qualité et sécurité
- Un étudiant = une branche et une PR par formation.
- Aucune modification du questionnaire, des consignes ou du travail des autres étudiants.
- Aucun mot de passe, token, clé SSH, donnée privée, capture de comptes sensibles.
- Ne pas exécuter de commandes destructrices sur une machine partagée ou en production.
- Les notes sont attribuées par le formateur, pas par une automatisation.
- Pour F03, F04..., reproduire le même chemin et remplacer `F02` par le code du module.

## Formateurs
Toute modification d'un support pédagogique passe par une branche `academy/...` et une PR administrative séparée. **Les PR de devoirs ne se fusionnent pas dans `main`** sauf décision expresse.
