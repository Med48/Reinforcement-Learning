**README - TP2 : Q-Learning sur FrozenLake**
**Description du TP**

Ce deuxième travail pratique (TP2) implémente l'algorithme Q-Learning pour résoudre l'environnement FrozenLake-v1 de Gymnasium, un problème classique de Reinforcement Learning.
Fichier

**TP2.ipynb**
**Objectif**

    Implémenter l'algorithme Q-Learning

    Entraîner un agent à naviguer dans l'environnement FrozenLake

    Évaluer les performances de l'agent

**Contenu détaillé**

    Initialisation de l'environnement :

        Création de l'environnement FrozenLake-v1 (mode glissant activé)

        Exploration des espaces d'actions et d'observations

    Initialisation de la Q-table :

        Création d'une table Q de dimensions (16 états × 4 actions)

        Initialisation avec des valeurs nulles

    Paramètres d'apprentissage :

        Taux d'apprentissage (alpha = 0.1)

        Facteur d'actualisation (gamma = 0.99)

        Taux d'exploration initial (epsilon = 1.0)

        Décroissance d'epsilon (epsilon_decay = 0.995)

        Nombre d'épisodes (5000)

    Algorithme Q-Learning :

        Phase d'exploration/exploitation (politique ε-gloutonne)

        Mise à jour des valeurs Q selon la formule :
        Copy

        Q(s,a) = Q(s,a) + α * (r + γ * max(Q(s',a')) - Q(s,a))

        Réduction progressive du taux d'exploration

    Évaluation des performances :

        Test sur 100 épisodes avec la politique apprise

        Calcul du taux de réussite (68% dans notre cas)

**Résultats attendus**

    Q-table remplie avec les valeurs apprises

    Taux de réussite d'environ 70% après entraînement

    Visualisation des valeurs Q pour chaque état-action

**Concepts clés**

    Apprentissage par renforcement tabulaire

    Politique ε-gloutonne

    Actualisation des valeurs Q

    Exploration vs exploitation

    Environnement à états discrets