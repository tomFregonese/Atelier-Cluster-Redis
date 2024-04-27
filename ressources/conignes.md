Atelier Cluster Redis

Partie 1: Installation et Configuration du Cluster Redis
Objectifs

    Créer un cluster Redis sur un seul serveur ou via Docker.
    Comprendre l'architecture de Redis et les principes de clustering.

Étapes à Réaliser

    Choix de l'Environnement :
        Décider si le cluster sera configuré sur un serveur unique ou dans des conteneurs Docker.

    Installation de Redis :
        Installer Redis localement ou via des images Docker.

    Configuration du Cluster :
        Configurer plusieurs instances de Redis pour qu'elles fonctionnent en mode cluster.

    Démarrage du Cluster :
        Lancer les instances Redis configurées pour former un cluster.

Restitution

    Documenter l'architecture choisie, les étapes réalisées et le code de déploiement du cluster Redis.


Partie 2: Premiers Pas avec le Cluster Redis
Objectifs

    Manipuler différents types de données stockées dans Redis.
    Comprendre les opérations de base et avancées avec Redis.

Étapes à Réaliser

    Injection de Données :
        Insérer des données de différents types dans Redis (Strings, Lists, Sets, Hashes, Sorted Sets).

    Requêtage des Données :
        Effectuer des opérations de lecture sur les données stockées, en utilisant divers critères selon le type de données.

Restitution

    Documenter les types de données utilisés, les commandes exécutées, et les résultats obtenus.


Partie 3: Intégration de Redis dans un Projet
Objectifs

    Utiliser Redis comme entrepôt de données et comme système de cache dans une application.

Étapes à Réaliser

    Projet d'Annuaire (optionnel) :
        Créer une application d'annuaire où les données sont stockées dans Redis.
        Développer un script qui mesure la taille d'une page web, stocke cette information dans Redis avec une durée de vie, et vérifie le cache avant de refaire une mesure.

    Intégration dans un Projet Existant :
        Si possible, intégrer Redis dans un projet existant, en utilisant Redis pour le stockage de données et/ou comme cache.

Restitution

    Présenter le projet réalisé, décrire l'utilisation de Redis, et expliquer les bénéfices observés.


Partie 4: Introspection sur l'Intégration de Redis
Objectifs

    Analyser l'impact potentiel de l'intégration de Redis dans des projets futurs.

Étapes à Réaliser

    Évaluation des Projets Actuels :
        Identifier des projets existants où Redis pourrait être intégré.
        Évaluer les avantages potentiels (performance, scalabilité, etc.).

Restitution

    Préparer une analyse détaillée sur les avantages de l'intégration de Redis dans différents types de projets.