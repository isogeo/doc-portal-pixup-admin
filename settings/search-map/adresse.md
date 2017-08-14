## Recherche par adresse \(géocodage\)

Le portail permet aux utilisateurs de chercher des données concernant une adresse.

### Fonctionnement

Le service de géocodage utilisé est [Nominatim](https://nominatim.openstreetmap.org/), qui repose sur la base de données ouverte d'OpenStreetMap. Fcontionnellement, voici le déroulé :

1. l'utilisateur entre une adresse dans le champ dédié du portail ;
2. la requête est envoyée à Nominatim qui renvoie un polygone ;
3. ce polygone est alors envoyé à l'API Isogeo pour filtrer les résultats selon l'opérateur géographique choisi \(voir Recherche géographique\)

### Options

#### Activer / désactiver

La première liste déroulante permet d'activer ou de désactiver le champ "Adresse" de l'interface utilisateur \(front-office\), sur la page d'accueil.

#### Encadrer la recherche

Le géocodage reste un processus automatique dont les résultats sont parfois fragiles selon le niveau d'exigence de l'utilisateur. L'écueil le plus courant est le problème d'homonymie. par exemple, la recherche "avenue charles de gaulle" a peu de chance de renvoyer exactement la bonne avenue si on ne donne pas plus de précisions au géocodeur.

C'est pour cela qu'il est fortement recommandé d'encadrer la recherche avec une emprise spatiale. Cette option correspond d'ailleurs à celle qui est proposée dans l'interface de [Nominatim](https://nominatim.openstreetmap.org/) \(_apply viewbox_\).

A noter que l'adresse email est utiliser pour identifier les requêtes auprès de l'infrastructure OpenStreetMap, au nom de [l'usage raisonnable de l'API de géocodage](https://operations.osmfoundation.org/policies/nominatim/) \(_fair-use_\).

![](/assets/back_search_geocoder.png)

