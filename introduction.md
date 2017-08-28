# Présentation générale du portail

Le portail présente 2 interfaces :

* celle visible par les utilisateurs, qu'ils soient authentifiés ou pas : c'est l'interface d'utilisation ou  front-office. Elle est souvent sur une URL du type : [http://_portail\_data_.domaine.com](http://_portail_data_.domaine.com_._).
* celle accessible uniquement aux administrateurs : c'est l'interface d'administration ou back-office. Elle est systématiquement sur l'adresse [http://portail\_data.domaine.com](http://portail_data.domaine.com)**/admin.**

Ce guide se concentre sur la deuxième, même si la première est utilisée pour illustrer les conséquences de la configuration du back-office.

## Concilier Data Management et design web {#docs-internal-guid-ab3644e3-f47e-003b-1b41-8a882bfb2893}

Dans la vision d’Isogeo, le catalogage n’est qu’une étape intermédiaire vers la diffusion et la valorisation des données. Faire des métadonnées n’est pas une fin en soi et les catalogues de données sont bien trop souvent des interfaces dédiées à des techniciens et loin de respecter les règles de l’ergonomie.

C’est pourquoi le portail allie l’expertise d’Isogeo en matière de gouvernance et de valorisation des données, la puissance de la plate-forme qui permet de servir les \(méta\)données via son API et le savoir-faire d’une agence de développement et de design web : [PixUp](http://www.pixup.com).

### Des portails orientés usages à portée de tous

L’objectif n’est pas de mettre un simple catalogue en consultation mais d’implémenter des fonctionnalités dédiées à l’animation autour du patrimoine de données : retours d’expériences, commentaires, suivi des modifications, comptes utilisateurs, etc.

Par ailleurs, il est possible de tirer parti de la modularité d’Isogeo et de servir un ou plusieurs portails selon les besoins. Par exemple dans le cas où vous avez besoin de diffuser certaines de vos données en interne d’une certaine façon et d’autres en externe d’une autre façon. C’est très facile à réaliser et tout à fait transparent d’un point de vue d'administration.

![&quot;Les données sont consommées et produites par différents types de personnes - L&apos;accès doit être simple pour tous&quot;](/assets/misc_data_people.png)

### Des fonctionnalités au service de la stratégie de diffusion

#### Moteur de recherche Isogeo

Le portail intègre évidemment toute la puissance du [moteur de recherche Isogeo](http://help.isogeo.com/fr/features/inventory/search.html) : filtres dynamiques, options de tri des résultats, pagination, etc. le tout dans une interface claire et proche des outils utilisés quotidiennement.

![&quot;Interface de recherche - Options de filtre et de tri&quot;](/assets/front_search_filters_catalog.png)

Voir :

* [option de tri des résultats par défaut](/settings/search-map/searchtext.md) ;
* [créer des thématiques personnalisées regroupant des données pour proposer des filtres pertinents](/homepage/thematics.md) ;

![&quot;Interface de recherche - Options de filtre et de tri&quot;](/assets/front_search_filters_catalog.png)

#### Une gestion de contenus dynamiques et statiques

Focalisé sur les données, le portail permet d'insérer les informations sur celles-ci dynamiquement à partir de l'inventaire Isogeo, notamment sur la page d'accueil. Au-delà des données, le portail  intègre un CMS \(_Content Management System_ ou SGC - Système de Gestion de Contenus\) et permet ainsi l'édition de contenus éditoriaux, comme sur WordPress par exemple :

* pages statiques ;
* gestion des rubriques et des menus ;
* gestionnaire d’actualités \(création, édition, publication, mise en avant en page d’accueil…\) ;
* gestionnaire de médias et de fichiers pour enrichir vos contenus facilement ;

![&quot;Articles et catégories - Exemple du SMAVD&quot;](/assets/front_news_smavd.png)

Voir :

* [gérer les pavés de flux dynamiques en page d'accueil](/homepage/dyn-sections.md) ;
* [créer une actualité](/actualites/newarticle.md) ;
* [créer une page statique](/pages/pageseditor.md) ;
* [utiliser l'éditeur de texte WYSIWYG](/appendices/editorwysiwyg.md).

#### Dimension géographique et interface cartographique

La dimension géographique est au coeur de l’expertise Isogeo et des fonctionnalités spécifiques sont intégrées pour la valoriser facilement :

* visualisation des services web géographiques \(WMS, WMTS, WFS, Esri Map, Esri Tiled Map, Esri Feature\) liés aux métadonnées de données, directement dans la fiche ;
* recherche par nom de lieux \(via le service de géocodage Nominatim lié au projet OpenStreetMap\) ;
* un filtre par des emprises géographiques personnalisables par l’administrateur via un fichier GeoJSON ;
* une interface cartographique de recherche est également disponible permettant de filtrer les résultats par localisation de leur emprise \(centroïde\).

![&quot;Interface cartographique de recherche - Aperçu d&apos;une métadonnée&quot;](/assets/front_map_metadata_modale.png)

Voir :

* [paramétrer l'interface cartographique et la recherche géographique](/settings/search-map/searchmap.md) ;
* [définir des emprises géographiques de recherche personnalisées](/settings/search-map/searchbbox.md) ;

### Une dimension participative pour servir l'animation autour du patrimoine immatériel

un espace et des options dédiés aux utilisateurs authentifiés :accéder à des pages réservées ou à des détails supplémentaires sur les fiches de métadonnées,accéder aux fonctionnalités participatives,création de listes de données personnalisées,

un outil de travail optimisé grâce aux notifications :un utilisateur peut choisir de s’abonner à certaines données \(via les listes\)toutes les semaines \(période personnalisable\), il reçoit un rapport par mail lui indiquant quelles données ont été modifiées entre temps sans aucune intervention de la part de l’administrateur.

partager ses listes aux autres utilisateurs, en public ou bien les garder privées,

* personnaliser l’affichage des informations \(par exemple, masquer / afficher systématiquement le tableau des attributs\)

Voir :

* [modérer les commentaires](/messages-recus/comment.md) ;
* [consulter les données évaluées](/stats/evaluations.md) ;

## Une administration simple mais puissante

L'interface d'administration, inspirée d'outils réputés tels WordPress, permet de gérer l'accès au portail mais aussi l'affichage des différents champs de métadonnées selon les types d'utilisateurs.

Voir :

* [rendre l'authentification au portail obligatoire](/settings/general.md) ;
* [gérer les utilisateurs](/users/user-management.md) ;
* [gérer l'affichage selon le type d'utilisateur](/settings/display.md).

### Un socle générique habillé de chartes graphiques personnalisées

le portail générique de démonstration \(parfois en travaux\) : [http://demo.isogeo.net](http://demo.isogeo.net) ;Créteil Géo Open Data : [http://geodata.ville-creteil.fr](http://geodata.ville-creteil.fr) ;Plaine Centrale Géo Open Data : [http://geodata.agglo-plainecentrale94.fr](http://geodata.agglo-plainecentrale94.fr) ;GéoLorient : [http://geocatalogue.lorient-agglo.bzh/](http://geocatalogue.lorient-agglo.bzh/) ;Grand Port Maritime de Nantes Saint-Nazaire \(privé\) [http://gpmnsn.isogeo.net](http://gpmnsn.isogeo.net) ;Syndicat Mixte d’Aménagement de la Vallée de la Durance \(privé\) [http://smavd.isogeo.net](http://smavd.isogeo.net) ;

### Un champ fonctionnel large, complet et cohérént

Beaucoup d’autres fonctionnalités viennent compléter l'expérience utilisateur :

* adapté à tous les formats de supports \(_responsive design_\) ;
* export des métadonnées au format PDF ;
* des statistiques pour le reporting de l'administrateur : généralistes \(Google Analytics\) et spécifiques \(vues, ressources, recherches, etc.\) ;
* un référencement optimisé pour les moteurs de recherche \(SEO\) ;
* lien direct vers l’édition de la fiche de métadonnées pour les éditeurs Isogeo ;
* interprétation du [langage Markdown](http://help.isogeo.com/fr/features/documentation/syntax_markdown.html) disponible dans Isogeo ;
* bouton pour copier le chemin d’une donnée fichier dans le presse-papiers directement depuis la métadonnée ;
* générer un code d’intégration iFrame à partir de chaque fiche de métadonnées ;



