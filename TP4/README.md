**README - TP4 : Algorithmes de Policy Gradient (PPO) pour Taxi-v3**
**Description du TP**

Ce quatrième travail pratique (TP4) implémente une version simplifiée de l'algorithme PPO (Proximal Policy Optimization) pour entraîner un agent dans l'environnement Taxi-v3 de Gymnasium.
Fichier

**TP4.ipynb**
**Objectif**

    Implémenter un algorithme de Policy Gradient (PPO)

    Comprendre les mécanismes d'optimisation des politiques

    Évaluer les performances sur l'environnement Taxi-v3

**Contenu détaillé**

**1. Initialisation de l'environnement**

    Création de l'environnement Taxi-v3

    Dimensions :

        Espace d'états : 500 états discrets

        Espace d'actions : 6 actions

**2. Structures de données**

    Table de politique :

        Initialisée uniformément (1/action_size)

        Représente π(a|s)

    Table de valeurs :

        Initialisée à 0

        Estime V(s)

**3. Paramètres d'apprentissage**

    γ = 0.99 (facteur d'actualisation)

    lr_policy = 0.1 (taux d'apprentissage)

    clip_epsilon = 0.2 (paramètre de clipping PPO)

    20 épisodes d'évaluation

**4. Algorithme PPO simplifié**

    Collecte de trajectoires :

        Exécution de la politique courante

        Stockage des (états, actions, récompenses)

    Calcul des récompenses actualisées :
    python
    Copy

    running_add = r + γ * running_add

        Normalisation des récompenses

    Mise à jour de la politique :

        Calcul du ratio des probabilités

        Fonction objectif PPO avec clipping :
    python
    Copy

    surr1 = ratio * advantage
    surr2 = clip(ratio, 1-ε, 1+ε) * advantage
    policy_loss = -min(surr1, surr2)

    Mise à jour des valeurs :

        Actualisation avec l'avantage calculé

**5. Évaluation des performances**

    20 épisodes de test

    Métriques :

        Récompense moyenne

        Taux de réussite

**Concepts clés**

    Méthodes de Policy Gradient

    Algorithmes de type Actor-Critic

    Mécanisme de clipping (PPO)

    Calcul d'avantage

    Normalisation des récompenses