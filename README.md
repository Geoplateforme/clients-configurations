Ce projet contient des configurations facilitant l'utilisation des services de la Géoplateforme. Les outils utilisés sont :

* [Bruno](https://www.usebruno.com/) comme client pour les API Rest (API Entrepôt, service de téléchargement...)
* [Insomnia](https://insomnia.rest/) comme client pour les API Rest (altimétrie...)
* [QGis](https://www.qgis.org/fr/site/) comme client de consommation des services de diffusion des données selon les standards OGC.

## Configuration QGis

* [Catalogue des serveurs WFS](./qgis/wfs.xml) (Points d'accès open et restreint, des environnements de production et de qualification)
* [Catalogue des serveurs WMS / WMTS](./qgis/wms-wmts.xml) (Points d'accès open et restreint, des environnements de production et de qualification)

## Configuration Insomnia

* [Utilisation du service d'altimétrie](./insomnia/diffusion/altimetrie.json)

## Collections Bruno

* [Alimentation et diffusion en téléchargement de données archives](./bruno/entrepot/archive/)

Pour utiliser la collection, il faut :

* Dans le dossier de la collection, exécuter `npm install` afin d'installer les librairies requises par les formulaires de demande d'identifiant.
* Ajouter le secret du client d'authentification :
    * `OqajgURfG9CfR7J16VogwyVSD85UXKNN` pour la qualification
    * `apQwgY9OvgOboNgBvGhxB7IgOqntoiEv` pour la production
* Jouer la requête `Connexion` afin de récupérer le token de votre compte
* Jouer la requête `Compte connecté` afin de récupérer la liste des communities et datastores dont vous êtes membres. Cela permettra d'avoir un menu déroulant lors du choix du datastore pour les requêtes d'alimentation
* Jouer la requête `Entrepôt courant` afin de récupérer la liste des points d'accès disponibles dans le datastore. Cela permettra d'avoir un menu déroulant lors de la publication d'une offre

Les identifiants nécessaires pour les requêtes seront en grande majorité remplis automatiquement au cours du workflow, ou demandé via des formulaires.