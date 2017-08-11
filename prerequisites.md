# Prérequis

## Isogeo

* au moins un groupe de travail Isogeo dans un abonnement payant
* au moins un catalogue contenant au moins une métadonnée, partagé à l'application ;
* des clés d'authentification auprès de l'API Isogeo ;

## Navigateurs supportés

* Google Chrome \(5 dernières versions\) ;
* Mozilla Firefox \(ESR et ultérieures\) ;
* Safari

## Connexion internet

---

# Environnement technique

## Spécifications serveur

* IIS
* connexion autorisée et configurée \(proxy, pare-feu...\) vers les domaines de l'API Isogeo :
  * [https://v1.api.isogeo.com/\*](https://v1.api.isogeo.com/)
  * [https://id.api.isogeo.com/\*](https://v1.api.isogeo.com/)
* accès à l'API nominatim : [https://nominatim.openstreetmap.org/](https://nominatim.openstreetmap.org/) ;

## Briques logicielles utilisées

* PHP version 5.6.13 ;
* MySQL 5.6.26 ;

## Eléments graphiques

Les différents éléments graphiques de personnalisation du portail sont livrés au format Photoshop \(.psd\) dans un fichier `icones et visuels.psd`, contenant les objets vectoriels répartis en plusieurs calques et groupes de calques :

![](/assets/tech_graphics_psd.png)

