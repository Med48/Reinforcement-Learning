**README - TP1 : Introduction à Gymnasium et CartPole**
**Description du TP**

Ce premier travail pratique (TP1) est une introduction à l'environnement CartPole-v1 de Gymnasium, conçu pour vous familiariser avec les concepts de base du Reinforcement Learning.
Fichier

**TP1.ipynb**
**Objectif**

**Prendre en main l'environnement CartPole-v1 en explorant :**

    L'espace d'actions et d'observations

    Les mécanismes de récompense

    L'interaction avec l'environnement

**Contenu détaillé**

    Initialisation de l'environnement :

        Création de l'environnement CartPole-v1

        Réinitialisation de l'environnement

    Exploration des espaces :

        Affichage de l'espace d'actions (2 actions possibles : gauche/droite)

        Affichage de l'espace d'observations (4 valeurs : position, vitesse, angle, vitesse angulaire)

    Exécution d'actions aléatoires :

        Simulation de 100 pas avec des actions aléatoires

        Affichage des observations et récompenses obtenues

        Réinitialisation lorsque l'épisode se termine

    Interaction manuelle :

        Mode permettant de saisir manuellement des actions (0 ou 1)

        Affichage en temps réel des observations

        Comptage du nombre d'étapes avant la fin de l'épisode

**Prérequis**

    Python 3.9+

    Bibliothèque Gymnasium

**Concepts clés abordés**

    Environnement Gymnasium

    Espace d'actions discret

    Espace d'observations continues

    Structure de base d'un épisode RL

    Récompenses immédiates