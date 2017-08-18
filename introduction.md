# Présentation générale du portail

Le portail présente toujours 2 interfaces :

* celle visible par les utilisateurs, qu'ils soient authentifiés ou pas : c'est l'interface d'utilisation ou  front-office. Elle est souvent sur une URL du type : http://_portail\_data_.domaine.com_._
* celle accessible uniquement aux administrateurs : c'est l'interface d'administration ou back-office. Elle est systématiquement sur l'adresse _http://portail\_data.domaine.com_**/admin.**

Ce guide se concentre sur la deuxième, même si la première est utilisée pour illustrer les conséquences de la configuration du back-office.



### Quand Data Management et design web font bon ménage {#docs-internal-guid-ab3644e3-f47e-003b-1b41-8a882bfb2893}

Dans la vision d’Isogeo, le catalogage n’est qu’une étape intermédiaire vers la diffusion et la valorisation des données. Faire des métadonnées n’est pas une fin en soi et les catalogues de données sont bien trop souvent des interfaces dédiées à des techniciens et loin de respecter les règles de l’ergonomie.

C’est pourquoi le portail allie l’expertise d’Isogeo en matière de gouvernance et de valorisation des données, la puissance de la plate-forme qui permet de servir les \(méta\)données via son API et le savoir-faire d’une agence de développement et de design web : [PixUp](http://www.pixup.com).

### Des portails orientés usages à portée de tous

L’objectif n’est pas de mettre un simple catalogue en consultation mais d’implémenter des fonctionnalités dédiées à l’animation autour du patrimoine de données : retours d’expériences, commentaires, suivi des modifications, comptes utilisateurs, etc. Par ailleurs, il est possible de tirer parti de la modularité d’Isogeo et de servir un ou plusieurs portails selon les besoins. Par exemple dans le cas où vous avez besoin de diffuser certaines de vos données en interne d’une certaine façon et d’autres en externe d’une autre façon. C’est très facile à réaliser et tout à fait transparent d’un point de vue d'administration.

### Des fonctionnalités au service de la stratégie de diffusion

#### Moteur de recherche Isogeo

Le portail intègre évidemment toute la puissance du [moteur de recherche Isogeo](http://help.isogeo.com/fr/features/inventory/search.html) : filtres dynamiques, options de tri des résultats, pagination, etc. le tout dans une interface claire et proche des outils utilisés quotidiennement.

Voir :

* [option de tri des résultats par défaut](/settings/search-map/searchtext.md) ;
* [créer des thématiques personnalisées regroupant des données pour proposer des filtres pertinents](/homepage/thematics.md) ;

![](/assets/front_search_filters_catalog.png)

#### Une gestion de contenus dynamiques et statiques

Des flux dynamiques sur l’actualité des données, tirant partie des différentes dates \(création dernière modification, etc.\) portant sur la donnée \(grâce au scan automatique notamment\) et sur la métadonnée.



Voir :

* [gérer les pavés de flux dynamiques en page d'accueil](/homepage/dyn-sections.md) ;
* [créer une actualité](/actualites/newarticle.md) ;
* [créer une page statique](/pages/pageseditor.md) ;
* [utiliser l'éditeur de texte WYSIWYG](/appendices/editorwysiwyg.md).

#### Dimension géographique et interface cartographique



![](/assets/front_map_metadata_modale.png)

Voir :

* [paramétrer l'interface cartographique et la recherche géographique](/settings/search-map/searchmap.md) ;
* [définir des emprises géographiques de recherche personnalisées](/settings/search-map/searchbbox.md) ;

### Une dimension participative pour servir l'animation autour du patrimoine immatériel







