**README - Travaux Pratiques en Reinforcement Learning**
**Description des TPs**

Ce dépôt contient quatre travaux pratiques (TPs) sur le Reinforcement Learning, couvrant différents algorithmes et environnements. Voici une description de chaque TP :
**TP1 : Introduction à Gymnasium et CartPole**

    Fichier: TP1.ipynb

    Objectif: Prise en main de l'environnement CartPole-v1 de Gymnasium.

    Contenu:

        Initialisation de l'environnement CartPole.

        Exploration de l'espace d'actions et d'observations.

        Exécution d'actions aléatoires et analyse des résultats.

        Interaction manuelle avec l'environnement pour comprendre les récompenses et les états.

**TP2 : Q-Learning sur FrozenLake**

    Fichier: TP2.ipynb

    Objectif: Implémentation de l'algorithme Q-Learning pour résoudre l'environnement FrozenLake.

    Contenu:

        Initialisation de l'environnement FrozenLake.

        Création et initialisation d'une Q-table.

        Entraînement de l'agent avec Q-Learning (paramètres ajustables : alpha, gamma, epsilon).

        Évaluation des performances de l'agent après entraînement.

        Affichage du taux de réussite.

**TP3 : Q-Learning vs SARSA sur un environnement de trafic**

    Fichier: TP3.ipynb

    Objectif: Comparaison des algorithmes Q-Learning et SARSA sur un environnement personnalisé de trafic.

    Contenu:

        Initialisation de l'environnement TrafficEnvironment.

        Implémentation de Q-Learning et SARSA avec des paramètres similaires pour une comparaison équitable.

        Visualisation des récompenses par épisode pour les deux algorithmes.

        Analyse des performances relatives.

**TP4 : Policy Gradient (PPO) sur Taxi-v3**

    Fichier: TP4.ipynb

    Objectif: Utilisation de l'algorithme PPO (Proximal Policy Optimization) pour entraîner un agent dans l'environnement Taxi-v3.

    Contenu:

        Initialisation des tables de politique et de valeurs.

        Simulation d'épisodes avec une politique aléatoire.

        Mise à jour de la politique avec PPO (incluant le calcul des récompenses actualisées et l'utilisation de "clipping").

        Évaluation des performances après entraînement (récompense moyenne et taux de réussite).

**Prérequis**

    Python 3.9+

    Bibliothèques requises :

        gymnasium

        numpy

        matplotlib (pour les visualisations dans TP3)

        traffic_env (environnement personnalisé pour TP3)

**Utilisation**

Exécutez les notebooks Jupyter dans l'ordre (TP1 à TP4) pour une progression logique des concepts. Chaque TP contient des commentaires détaillés et des explications.

**Auteur**

    Mohammed Rhouati