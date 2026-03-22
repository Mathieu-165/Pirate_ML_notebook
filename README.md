# Projet PIRATE ML - 3A ESTACA

**Auteurs :** GRANGER M., LEVERS G.

L'objectif de ce projet est d'étudier l'impact potentiel du Machine Learning dans le traitement de données d'essais mécaniques pour l'optimisation de structures. 

Plus précisément, ce dépôt contient un notebook permettant de prédire et classifier des éprouvettes en fonction de leur module de flexion, calculé à partir d'un essai de flexion en 3 points (selon la norme **NF EN ISO 14125**).

## ✨ Fonctionnalités et Modèles

*   **Analyse exploratoire** : Visualisation de la répartition et de la densité des modules d'Young (Violin plots), et étude des corrélations des caractéristiques géométriques et d'efforts.
*   **Modélisation ML** : Entraînement et comparaison de 3 modèles régressifs via un pipeline complet :
    *   SVR (Support Vector Regression)
    *   k-NN (k-Nearest Neighbors)
    *   Random Forest
*   **Optimisation** : Recherche des meilleurs hyperparamètres pour chaque modèle à l'aide de `GridSearchCV`.
*   **Évaluation** : Calcul des performances (RMSE, R²) et tracé de matrices de confusion.
*   **Explicabilité (SHAP)** : Analyse de l'impact des variables sur les prédictions du modèle SVR (graphiques globaux et locaux).
*   **Déploiement** : Exportation du meilleur modèle au format `.pkl` prêt à être réutilisé.

## 📂 Structure du projet

*   `notebook_ml.ipynb` : Le notebook principal contenant l'intégralité de l'étude (traitement, entraînement, explicabilité).
*   `notebook_generation_data.ipynb` : Le notebook chargé de la génération des jeux de données d'essais simulés.
*   `data/` : Dossier contenant les jeux de données d'essais simulés (`.csv`).
*   `model_export/` : Dossier contenant les modèles entraînés sauvegardés (ex: `modele_svr_final.pkl`).
*   `requirements.txt` : La liste exacte des dépendances Python nécessaires pour faire tourner le projet.

## 🚀 Quickstart (Installation Rapide)

**1. Cloner le dépôt :**
```bash
git clone https://github.com/Mathieu-165/Pirate_ML_notebook.git
```

**2. Créer et activer l'environnement virtuel (.venv) :**
```bash
# Sur Windows
python -m venv .venv
.venv\Scripts\activate

# Sur Mac/Linux
python3 -m venv .venv
source .venv/bin/activate
```

**3. Installer les dépendances :**
```bash
pip install -r requirements.txt
```

## 🚀 Utilisation
1. Ouvrez le fichier `notebook_ml.ipynb` dans VS Code.
2. En haut à droite, cliquez sur "Select Kernel" > "Python Environments" et choisissez l'environnement `.venv` que vous venez de créer.
3. Exécutez les cellules !