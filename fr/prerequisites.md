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

## Connexion Internet {#internet}

En mode SaaS, un débit descendant minimum de **500 Kb/s** est requis pour accéder au Portail.

## Services géographiques pris en charge {#services}

Le Portail permet l'exploitation des couches de services cartographiques ouverts pour visualiser les données. Les services suivants peuvent être exploités :

* les services de type Feature issues d'un service OGC, WFS ou Esri, Esri Feature Service
* les services de type Map issues d'un service OGC, WMS, ou Esri, Esri Map Service

> NB : En mode On-premises, les services doivent être accessibles sur la machine hébergeant le Portail. 

Les groupes de couche ne sont pas actuellement pris en compte, seules les couches sont exploitables. 

## Autres (optionnels mais recommandés) {#others}

* [Accès au portail en HTTPS sur un domaine et avec un certificat de l'organisme client](/appendices/https.md)
* [Configuration du serveur de mail de l'organisme client](/settings/general.md#mail_server)
* Authentification des utilisateurs au Portail en SSO avec [AzureAD](/appendices/azuread.md) ou Okta.

<!-- ---

## Environnement technique {#environment}

Généralement, le portail est hébergé par Isogeo en SaaS, mais celui-ci peut également être déployé en interne selon les prérequis ci-dessous. 

### Spécifications serveur

* Serveur web compatible avec PHP (Windows/IIS, Linux/Apache) et MySQL ou PostgreSQL au besoin
* connexion autorisée et configurée \(proxy, pare-feu...\) vers les domaines de l'API Isogeo :
  * [https://v1.api.isogeo.com/\*](https://v1.api.isogeo.com/)
  * [https://id.api.isogeo.com/\*](https://v1.api.isogeo.com/)
* Cache applicatif activé

### Briques logicielles utilisées {#softwares}

* PHP : version 7.1+ ; 
* MySQL 5.7+ ou PostgreSQL 11+ ;
* [Helicon ISAPI Rewrite](http://www.helicontech.com/isapi_rewrite/) pour la gestion des fichiers *.htaccess* sur les serveurs IIS uniquement. -->