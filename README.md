## Pré-requis
Pour installer l'application dans votre environnement, vous devez avoir :
 - Composer dernière version installé dans votre serveur
 - PHP version supérieur ou égale 8.1
 - Mysql

## Importation du code source
Il vous faut télécharger le code source de l'application sur le dépôt git ou utiliser la commande "git clone +lien_github" dans un terminal dans votre environnement.

## Installation des dépendances
Pour installer les dépendances de l'application sur votre serveur, il suffit de lancer la commande "composer install" dans un terminal dans le dossier racine du projet.

## Mise en place de la base de données
- Créer une base de données dans mysql et ajouter les informations de connexion dans le fichier ".env"(qui se trouve dans la racine du projet) : 
    DB_HOST=ADRESSE_DE_VOTRE_MACHINE (127.0.0.1 pour le local)
    DB_PORT=PORT_MYSQL (3306 par défaut)
    DB_DATABASE=NOM_DE_LA_BASE_DE_DONNEES
    DB_USERNAME=UTILISATEUR_AYANT_DES_DROITS_SUR_LA_BDD
    DB_PASSWORD=MOT_DE_PASSE
- Importer toutes les tables qui se trouve dans le fichier "db/structure.sql" en copiant tous les scripts pour la création des tables dans la base de données.
- Importer toutes les données des tables qui se trouve dans le fichier "db/donnees.sql" en copiant tous les scripts pour importer les données de chaques tables de la base de données.

## Lancer l'application
Ouvrir un terminal dans la racine du projet et lancer la commmande "php artisan serve"

## Compte administrateur par défaut
Adresse mail : admin@admin.com
Mot de passe : admin

Pour créer d'autre compte administrateur, il faut vous connecter en tant qu'administrateur avec ce compte dans le site et de rajouter dans le menu "Gestion de compte/Ajout compte admin" dans la partie administration du site.

## Administration
Dans la partie administration, vous pouvez : 
- Visualiser, ajouter et annuler les réseravtions envoyées par les clients
- Modifier les horaires journalier
- Modifier la carte ou les menus
- Modifier les images sur la gallerie dans la page d'accueil du site
- Modifier la limite de réservation pour les services 

## Partie client
Sur le site, vous pouvez :
- Créer un compte
- Réserver une table à un date précise
- Consulter et annuler vos réservations
