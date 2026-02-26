# Projet PIRATE ML 3A ESTACA - GRANGER M., LEVERS G.

Ce projet contient un notebook ayant pour objectif la classification d'éprouvettes en fonction de leur module de flexion. Pour cela il utilise 3 modèles de Machine Learning : SVR, KNN, Random Forest.

## 🛠️ Installation et Configuration (Pour les collaborateurs)

Pour faire tourner ce projet en local sur votre machine, suivez ces étapes :

**1. Cloner le projet**
Récupérez le code sur votre ordinateur via Git :
`git clone https://github.com/Mathieu-165/Pirate_ML_notebook`

**2. Créer l'environnement virtuel**
Ouvrez le dossier du projet dans VS Code, ouvrez un terminal ("Terminal" > "New terminal") et créez une "boîte isolée" pour les bibliothèques :
* Sur Windows : `python -m venv .venv`
* Sur Mac/Linux : `python3 -m venv .venv`

**3. Activer l'environnement**
* Sur Windows : `.venv\Scripts\activate`
* Sur Mac/Linux : `source .venv/bin/activate`
*(Vérifiez qu'un petit `(.venv)` vert apparaît au début de votre ligne de commande).*

**4. Installer les dépendances**
Installez toutes les bibliothèques nécessaires (scikit-learn, pandas, etc.) en une seule commande grâce à la recette :
`pip install -r requirements.txt`

## 🚀 Utilisation
1. Ouvrez le fichier `notebook_v4.ipynb` dans VS Code.
2. En haut à droite, cliquez sur "Select Kernel" > "Python Environments" et choisissez l'environnement `.venv` que vous venez de créer.
3. Exécutez les cellules !