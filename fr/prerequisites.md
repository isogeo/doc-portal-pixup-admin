# Prérequis

## Isogeo

* au moins un groupe de travail Isogeo ;
* au moins un catalogue contenant au moins une métadonnée, partagé à l'application ;
* des clés d'authentification auprès de l'API Isogeo ;

## Navigateurs supportés

* Google Chrome \(5 dernières versions\) ;
* Mozilla Firefox \(ESR et ultérieures\) ;
* Safari ;
* Edge.

---

# Environnement technique

## Spécifications serveur

* IIS 
* connexion autorisée et configurée \(proxy, pare-feu...\) vers les domaines de l'API Isogeo :
  * [https://v1.api.isogeo.com/\*](https://v1.api.isogeo.com/)
  * [https://id.api.isogeo.com/\*](https://v1.api.isogeo.com/)
* accès à l'API nominatim : [https://nominatim.openstreetmap.org/](https://nominatim.openstreetmap.org/) ;

### Configuration idéale

* Machine physique dédiée
* Processeur Xeon D1521 2.40 Ghz \(x8\)
* Système d’exploitation Windows Server 2012 R2 ou 2016
* IIS v8.5
* Mémoire 32 Go
* Disque dur 2x2 To + 2 x 300 Go SSD
* Cache applicatif activé

## Briques logicielles utilisées

* PHP version 5.6.13 ou 7.x ;
* MySQL 5.6.26 ;
* [Helicon ISAPI Rewrite](http://www.helicontech.com/isapi_rewrite/) \(pour la gestion des fichiers .htaccess\).

## Eléments graphiques

Les différents éléments graphiques de personnalisation du portail sont livrés au format Photoshop \(.psd\) dans un fichier `icones et visuels.psd`, contenant les objets vectoriels répartis en plusieurs calques et groupes de calques :

![&quot;Aperçu des calques Photoshop dans le fichier tranmis&quot;](/assets/tech_graphics_psd.png)

