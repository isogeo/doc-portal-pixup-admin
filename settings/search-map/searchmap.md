## Recherche géographique et interface cartographique

### Fonctionnement

La dimension géographique est utilisée principalement dans deux fonctionnalités dans le portail :

* lors de la recherche par emprises personnalisées ;
* dans l'interface de recherche cartographique ;

C'est dans cette partie du back-office que l'administrateur peut régler l'ensemble des paramètres liés aux fonctionnalités à dimension géographique.

![](/assets/back_search_map.png)

### Options

#### Activer / désactiver l'interface cartographique

Si l'option est activée :

* le menu "Carte" est ajouté à la barre du menu horizontal du portail ;
* l'interface de recherche cartographique est accessible à l'adresse http://\[URL\_PORTAIL\]**/carto ;**
* les autres options sont disponibles ;

Si l'option est désactivée :

* http://\[URL\_PORTAIL\]**/carto** affiche un message indiquant que le module est désactivé :

![](/assets/front_map_disabled.PNG)

* les autres options sont masquées dans le back-office.

#### Niveaux de zooms

Il est possible de régler le zoom minimum et maximum.

Ces options permettent d'éviter que l'utilisateur ne zoom ou ne dézoome trop sur la cart, perturbant les recherches via les enveloppes convexes des données.

#### Relation géométrique





#### Mise à jour de la liste carto



3 options sont possibles :

* Non : la liste des résultats de l'interface cartographique n'est pas rafraîchie à chaque changement d'emprise \(zoom ou déplacement\) ;
* Oui / basé sur la position des centroïdes \(plus rapide\) :
* Oui / basé sur les appels à l'API \(plus précis\) :

#### Fonds de carte

Sélectionnez les fonds de carte que vous souhaitez utiliser dans le module cartographique. Si plusieurs fonds sont cochés, l'utilisateur pourra choisir le fond qu'il souhaite utiliser. 

![](/assets/front_map_basemap_picker.png)

Si aucun fond n'est coché, le fond `OpenStreetMap : HOT` sera utilisé par défaut.

##### Ajouter un fond de carte personnalisé

Il est possible de permettre à l'utilisateur d'utiliser un de vos géoservices comme fond de carte. Il faut alors choisir le type de service web à utiliser, ainsi que l'URL vers la couche concernée.



