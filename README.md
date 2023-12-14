Ce projet contient des configurations facilitant l'utilisation des services de la Géoplateforme. Les outils utilisés sont :

* [Insomnia](https://insomnia.rest/) comme client pour les API Rest (API Entrepôt, altimétrie...)
* [QGis](https://www.qgis.org/fr/site/) comme client de consommation des services de diffusion des données selon les standards OGC.

## Configuration QGis

* [Catalogue des serveurs WFS](./qgis/wfs.xml) (Points d'accès open et restreint, des environnements de production et de qualification)
* [Catalogue des serveurs WMS / WMTS](./qgis/wms-wmts.xml) (Points d'accès open et restreint, des environnements de production et de qualification)

## Configuration Insomnia

* [Utilisation du service d'altimétrie](./insomnia/diffusion/altimetrie.json)