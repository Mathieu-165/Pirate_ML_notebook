## **Guide d'Onboarding : Projet PIRATE ML**

Bienvenue sur le projet ! Pour que l'on puisse coder ensemble sans risquer de casser nos ordinateurs respectifs ou d'avoir des conflits de versions, nous allons utiliser un environnement de développement standardisé.

**Ne saute aucune étape, surtout celles marquées d'un 🚨 !**

**---**

##### **Phase 1 : Création des comptes**

1. **Créer un compte GitHub :** Rends-toi sur [github.com](https://github.com/) et crée un compte (si tu n'en as pas déjà un).
2. **Débloquer GitHub Education (Bonus étudiant) :** Va sur [education.github.com/pack](https://education.github.com/pack)
   Connecte-toi avec ton adresse mail étudiante (en `@estaca.eu`)
   Cela te donnera accès gratuitement à GitHub Pro, ainsi qu'à GitHub Copilot (l'IA qui aide à coder directement dans l'éditeur) et plein d'autres outils professionnels.
3. **Accepter l'invitation :** une fois ton compte créée je t'enverrai une invitation pour rejoindre le dépôt privé du projet. Clique sur le lien dans l'e-mail pour l'accepter.

**---**

##### **Phase 2 : Installation de l'Arsenal (Logiciels)**

1. **Python** 🚨 (L'étape la plus critique)

   Va sur [python.org](https://www.python.org/downloads/) et télécharge la dernière version.
   ⚠ ATTENTION LORS DE L'INSTALLATION SUR WINDOWS : Sur la toute première fenêtre de l'installateur, tu dois absolument cocher la case en bas : "**Add Python to PATH**" (ou "Ajouter Python.exe au PATH"). Si tu oublies ça, rien ne marchera par la suite.
   Clique ensuite sur "Install Now".
2. **Visual Studio Code (VS Code)**
   C'est notre éditeur de code. Télécharge-le sur [code.visualstudio.com](https://code.visualstudio.com/) et installe-le.
3. **GitHub Desktop (Fortement recommandé)**
   C'est une interface visuelle très pratique pour ne pas avoir à taper des lignes de commande complexes pour récupérer ou envoyer le code.
   Télécharge-le sur [desktop.github.com](https://github.com/apps/desktop)
 	Ouvre-le et connecte-toi avec ton compte GitHub.

**---**

##### **Phase 3 : Préparer VS Code**

Ouvre VS Code. Sur la barre tout à gauche, clique sur l'icône des Extensions (les 4 petits carrés, ou `Ctrl+Shift+X`).
Recherche et installe ces deux extensions officielles publiées par Microsoft :
   * Python
   * Jupyter

**---**

##### **Phase 4 : Récupérer le projet (Le Clone)**

1. Ouvre GitHub Desktop.
2. Va dans "File" > "Clone repository…" (ou clique sur le bouton bleu "**Clone a repository**").
3. Dans l'onglet GitHub.com, cherche notre projet "**Pirate_ML_notebook**".
4. Choisis où tu veux le sauvegarder sur ton PC (ex: C:\\Users\\TonNom\\Documents\\Projets\\) et clique sur "Clone".
5. Une fois terminé, clique sur le bouton "**Open in Visual Studio Code**".

**---**

##### **Phase 5 : La Magie de l'Environnement Virtuel (Le .venv)**

Pour ne pas polluer ton PC avec les lourdes bibliothèques de Machine Learning, on va créer une "boîte isolée" juste pour ce projet.

1. Dans VS Code, ouvre le terminal intégré (Terminal > Nouveau terminal ou Ctrl+ù).
2. **Créer la boîte :** Tape la commande suivante et fais Entrée :
   *Sur Windows* : `python -m venv .venv`
   *Sur Mac/Linux* : `python3 -m venv .venv`
   (Un dossier `.venv` va apparaître à gauche, n'y touche pas manuellement).
3. **Activer la boîte 🚨 :**
   *Sur Windows* : `.venv\\Scripts\\activate`
   *Sur Mac/Linux* : `source .venv/bin/activate`
   **Important (Bug Windows) :** Si Windows t'affiche une erreur rouge disant que l'exécution de scripts est désactivée (UnauthorizedAccess), tape cette commande :
   	`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`, dis Oui (O), puis relance la commande d'activation.
   **Succès :** Tu dois voir (.venv) écrit en vert au début de la ligne de ton terminal.
4. **Installer les ingrédients :**
      Maintenant que l'environnement est activé, installe exactement les mêmes versions des bibliothèques que moi grâce à notre recette magique :
    	`pip install -r requirements.txt`
      Laisse tourner (ça peut prendre 1 à 2 minutes).

**---**

##### **Phase 6 : Lancer le Machine Learning ! 🚀**   

1. Toujours dans VS Code, ouvre notre fichier principal (`notebook_ml.ipynb`).
2. En haut à droite de l'écran, tu verras un bouton "**Select Kernel**" (ou la version de Python). Clique dessus.
3. Choisis "**Python Environments**"**.**
4. Sélectionne celui qui s'appelle **Python X.X.X ('.venv': venv)** (il y a souvent une petite étoile ★ à côté).
5. Lance la première cellule de code (Shift + Entrée). Si aucun message d'erreur n'apparaît, ton PC est officiellement une station de Data Science !

**Bienvenue à bord !**

