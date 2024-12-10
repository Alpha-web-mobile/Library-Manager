# Library-Manager
Application de Gestion de Bibliothèque
Description
Cette application web permet de gérer une bibliothèque. Elle permet de gérer des livres, leurs auteurs et les emprunts par les utilisateurs. L'application est développée en Symfony et utilise Doctrine pour la gestion des entités.

Installation
Cloner le dépôt

bash
git clone https://github.com/votre-utilisateur/library-management.git
cd library-management
Installer les dépendances

bash
composer install
Configurer la base de données

Modifier le fichier .env pour configurer la connexion à votre base de données :

env
DATABASE_URL="mysql://username:password@127.0.0.1:3306/library_management"
Créer la base de données et les schémas

bash
php bin/console doctrine:database:create
php bin/console doctrine:schema:update --force
Lancer le serveur de développement

bash
symfony server:start
L'application sera accessible à l'adresse http://127.0.0.1:8000.

Fonctionnalités
Gestion des livres : Ajouter, modifier, supprimer et rechercher des livres.

Gestion des auteurs : Ajouter, modifier et supprimer des auteurs.

Gestion des emprunts : Permettre aux utilisateurs d’emprunter des livres et visualiser les emprunts en cours.

Gestion des utilisateurs : Ajouter et gérer des utilisateurs avec des rôles différents (administrateur ou utilisateur standard).

Sécurité
L'application utilise le système de sécurité de Symfony pour gérer l'authentification et les autorisations. Les actions de création, modification et suppression sont réservées aux administrateurs.

Style
L'application utilise Bootstrap pour le style afin de simplifier la création d'une interface utilisateur.
