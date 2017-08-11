# Recherche et de l'interface cartographique

Dans cette partie, il est possible de régler l'ensemble des paramètres liés aux fonctionnalités de recherche du portail :

* la recherche textuelle ;
* la recherche par géocodage ;
* la recherche par emprise personnalisée ;
* la recherche via l'interface cartographique.

![](/assets/front_search_modes.png)

---

## Recherche textuelle

Lorsqu'un utilisateur entre des termes de recherche dans le champ de recherche, les résultats sont affichés dans selon le paramètres défini par l'administrateur dans cette partie parmi les valeurs suivantes :

* nom, par ordre alphabétique \(valeur par défaut\) ;
* date de modification des métadonnées ;
* date de création des métadonnées ;
* date de modification des données \(ressources\) ;
* date de création des données \(ressources\).

![](/assets/back_search_text_filter.PNG)

Il faut garder à l'esprit que :

* l'utilisateur peut de toute façon changer cette valeur via l'interface de recherche dans la page des résultats ;
* l'ordre de tri \(ascendant / descendant, alphabétique ou inverse\) est aussi réglable par l'utilisateur, mais pas par l'administrateur ;
* les dates de création et de modification des données \(ressources\) ne sont pas systématiquement renseignées. A ce sujet, consulter [l'annexe dans l'aide de la plateforme Isogeo](http://help.isogeo.com/fr/appendices/different_dates.html) ;
* les caractéristiques du moteur de recherche sont celles d'Isogeo, [documenté de façon détaillée ici](http://help.isogeo.com/fr/features/inventory/search.html) ;
* le champ de recherche textuelle ne peut être désactivé.

---

## Recherche par adresse \(géocodage\)

Le portail permet aux utilisateurs de chercher des données concernant une adresse.

### Fonctionnement

Le service de géocodage utilisé est Nominatim, qui 

### Options

La première liste déroulante permet d'activer ou de désactiver le champ "Adresse" de l'interface utilisateur (front-office), sur la page d'accueil.

![](/assets/back_search_geocoder.png)





