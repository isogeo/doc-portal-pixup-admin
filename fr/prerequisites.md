# Prérequis

## Isogeo

* au moins un groupe de travail Isogeo ;
* au moins un catalogue contenant au moins une métadonnée, partagé à l'application ;
* des clés d'authentification auprès de l'API Isogeo ;

## Navigateurs recommandés

* Google Chrome \(5 dernières versions\) ;
* Mozilla Firefox \(ESR et ultérieures\) ;
* Safari ;
* Edge.

---

# Environnement technique

## Spécifications serveur

* Serveur web compatible avec PHP (IIS, Apache) et MySQL
* connexion autorisée et configurée \(proxy, pare-feu...\) vers les domaines de l'API Isogeo :
  * [https://v1.api.isogeo.com/\*](https://v1.api.isogeo.com/)
  * [https://id.api.isogeo.com/\*](https://v1.api.isogeo.com/)
<!-- * accès à l'API nominatim : [https://nominatim.openstreetmap.org/](https://nominatim.openstreetmap.org/) ; -->

### Configuration idéale

* Machine physique dédiée
* Processeur Xeon D1521 2.40 Ghz (x8)
* Mémoire 32 Go
* Disque dur 2x2 To + 2 x 300 Go SSD
* Cache applicatif activé

Si environnement Microsoft

* Système d’exploitation Windows Server 2012 R2, 2016, 2019
* IIS minimum v8.5

## Briques logicielles utilisées

* PHP : version 7.x minimum ; 
* MySQL 5.6.26 ;
* [Helicon ISAPI Rewrite](http://www.helicontech.com/isapi_rewrite/) pour la gestion des fichiers *.htaccess* sur les serveurs IIS uniquement.