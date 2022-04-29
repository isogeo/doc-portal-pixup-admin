---
description: Pré-requis techniques du portail Isogeo
---
# Prérequis

## Isogeo {#isogeo}

Un paramétrage de la plateforme Isogeo est nécéssaire, il faut : 

* au moins un groupe de travail Isogeo ;
* au moins un catalogue contenant au moins une métadonnée, partagé à l'application ;
* des clés d'authentification auprès de l'API Isogeo ;

Ce paramétrage est généralement réalisé par l'équipe Isogeo.

## Navigateurs recommandés {#navigators}

* Google Chrome \(5 dernières versions\) ;
* Mozilla Firefox \(ESR et ultérieures\) ;
* Safari ;
* Edge.

---

## Environnement technique {#environment}

### Spécifications serveur

* Serveur web compatible avec PHP (Windows/IIS, Linux/Apache) et MySQL ou PostgreSQL au besoin
* connexion autorisée et configurée \(proxy, pare-feu...\) vers les domaines de l'API Isogeo :
  * [https://v1.api.isogeo.com/\*](https://v1.api.isogeo.com/)
  * [https://id.api.isogeo.com/\*](https://v1.api.isogeo.com/)
* Cache applicatif activé

### Briques logicielles utilisées {#softwares}

* PHP : version 7.1+ ; 
* MySQL 5.7+ ou PostgreSQL 11+ ;
* [Helicon ISAPI Rewrite](http://www.helicontech.com/isapi_rewrite/) pour la gestion des fichiers *.htaccess* sur les serveurs IIS uniquement.