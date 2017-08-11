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

Le service de géocodage utilisé est [Nominatim](https://nominatim.openstreetmap.org/), qui repose sur la base de données ouverte d'OpenStreetMap. Fcontionnellement, voici le déroulé :

1. l'utilisateur entre une adresse dans le champ dédié du portail ;
2. la requête est envoyée à Nominatim qui renvoie un polygone ;
3. ce polygone est alors envoyé à l'API Isogeo pour filtrer les résultats selon l'opérateur géographique choisi

### Options

#### Activer / désactiver

La première liste déroulante permet d'activer ou de désactiver le champ "Adresse" de l'interface utilisateur \(front-office\), sur la page d'accueil.

#### Encadrer la recherche

Le géocodage reste un processus automatique dont les résultats sont parfois fragiles selon le niveau d'exigence de l'utilisateur. L'écueil le plus courant est le problème d'homonymie. par exemple, la recherche "avenue charles de gaulle" a peu de chance de renvoyer exactement la bonne avenue si on ne donne pas plus de précisions au géocodeur.

C'est pour cela qu'il est fortement recommandé d'encadrer la recherche avec une emprise spatiale. Cette option correspond d'ailleurs à celle qui est proposée dans l'interface de [Nominatim](https://nominatim.openstreetmap.org/) \(_apply viewbox_\).

A noter que l'adresse email est utiliser pour identifier les requêtes auprès de l'infrastructure OpenStreetMap, au nom de [l'usage raisonnable de l'API de géocodage](https://operations.osmfoundation.org/policies/nominatim/) \(_fair-use_\).

![](/assets/back_search_geocoder.png)

