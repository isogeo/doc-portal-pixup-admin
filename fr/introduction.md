# Présentation générale du portail

Le portail présente 2 interfaces :

* celle visible par les utilisateurs, qu'ils soient authentifiés ou pas : c'est l'interface d'utilisation ou  front-office. Elle est souvent sur une URL du type : [http://_portail\_data_.domaine.com](http://_portail_data_.domaine.com_._).
* celle accessible uniquement aux administrateurs : c'est l'interface d'administration ou back-office. Elle est systématiquement sur l'adresse [http://portail\_data.domaine.com](http://portail_data.domaine.com)**/admin.**

Ce guide se concentre sur la deuxième, même si la première est utilisée pour illustrer les conséquences de la configuration.

## Concilier Data Management et design web {#docs-internal-guid-ab3644e3-f47e-003b-1b41-8a882bfb2893}

Dans la vision d’Isogeo, le catalogage n’est qu’une étape intermédiaire vers la diffusion et la valorisation des données. Faire des métadonnées n’est pas une fin en soi et les catalogues de données sont bien trop souvent des interfaces dédiées à des techniciens et loin de respecter les règles de l’ergonomie.

C’est pourquoi le portail allie l’expertise d’Isogeo en matière de gouvernance et de valorisation des données, la puissance de la plate-forme qui permet de servir les \(méta\)données via son API et le savoir-faire d’une agence de développement et de design web : [PixUp](http://www.pixup.com).

### Des portails orientés usages à portée de tous

L’objectif n’est pas de mettre un simple catalogue en consultation mais d’implémenter des fonctionnalités dédiées à l’animation autour du patrimoine de données : retours d’expériences, commentaires, suivi des modifications, comptes utilisateurs, actualités, mise en valeur du SIG etc.

Par ailleurs, il est possible de tirer parti de l'API Isogeo et de proposer un portail selon le profil d'utilisateur. Par exemple, si vous souhaitez diffuser certaines données qu'en interne et non en externe, c’est très facile à réaliser depuis l'administration.

![&quot;Les données sont consommées et produites par différents types de personnes - L&apos;accès doit être simple pour tous&quot;](/assets/misc_data_people.png)

### Au service de la stratégie de diffusion

#### Moteur de recherche Isogeo

Le portail intègre évidemment toute la puissance du [moteur de recherche Isogeo](http://help.isogeo.com/fr/features/inventory/search.html) : filtres dynamiques, options de tri des résultats, pagination, etc. le tout dans une interface claire et proche des outils utilisés quotidiennement.

![&quot;Interface de recherche - Options de filtre et de tri&quot;](/assets/front_search_filters_catalog.png)


#### Une gestion de contenus dynamiques et statiques

Le portail n'est pas uniquement focalisé sur les données. En effet, le portail intègre un CMS \(_Content Management System_ ou SGC - Système de Gestion de Contenus\) et permet ainsi l'édition de contenus éditoriaux, comme par exemple :

* gestion des menus ;
* gestionnaire d’actualités \(création, édition, publication, mise en avant en page d’accueil…\) ;
* gestionnaire de médias et de fichiers pour enrichir vos contenus facilement ;

![&quot;Articles et catégories - Exemple du SMAVD&quot;](/assets/front_news_smavd.png)

Voir :

* [gérer les pavés de flux dynamiques en page d'accueil](/homepage/dyn-sections.md) ;
* [créer une actualité](/actualites/newarticle.md) ;
* [créer une page statique](/pages/pageseditor.md) ;
* [utiliser l'éditeur de texte WYSIWYG](/appendices/editorwysiwyg.md).

<!-- #### Dimension géographique et interface cartographique

La dimension géographique est au coeur de l’expertise Isogeo et des fonctionnalités spécifiques sont intégrées pour la valoriser facilement :

* visualisation des services web géographiques \(WMS, WMTS, WFS, Esri Map, Esri Tiled Map, Esri Feature\) liés aux métadonnées de données, directement dans la fiche ;
* recherche par nom de lieux \(via le service de géocodage Nominatim lié au projet OpenStreetMap\) ;
* un filtre par des emprises géographiques personnalisables par l’administrateur via un fichier GeoJSON ;
* une interface cartographique de recherche est également disponible permettant de filtrer les résultats par localisation de leur emprise \(centroïde\).

![&quot;Interface cartographique de recherche - Aperçu d&apos;une métadonnée&quot;](/assets/front_map_metadata_modale.png)

Voir :

* [paramétrer l'interface cartographique et la recherche géographique](/settings/search-map/searchmap.md) ;
* [définir des emprises géographiques de recherche personnalisées](/settings/search-map/searchbbox.md) ; -->

### Dimension participative pour animer le patrimoine immatériel

Un espace et des options sont dédiées aux utilisateurs authentifiés : accéder à des pages réservées ou à des détails supplémentaires sur les fiches de métadonnées, accéder aux fonctionnalités participatives, créer dse listes de données personnalisées...

Un outil de travail optimisé grâce aux notifications : un utilisateur peut choisir de s’abonner à certaines données \(via les listes\) toutes les semaines \(période personnalisable\) il reçoit un rapport par mail lui indiquant quelles données ont été modifiées entre temps sans aucune intervention de la part de l’administrateur.

Partager ses listes aux autres utilisateurs, en public ou bien les garder privées,

* personnaliser l’affichage des informations \(par exemple, masquer / afficher systématiquement le tableau des attributs\)

Voir :

* [modérer les commentaires](/messages-recus/comment.md) ;
* [consulter les données évaluées](/stats/evaluations.md) ;
* [paramétrer les emails](/settings/emails.md) ;

## Une administration simple mais puissante

L'interface d'administration permet de gérer l'accès au portail mais aussi l'affichage des différents champs de métadonnées selon les types d'utilisateurs.

Voir :

* [rendre l'authentification au portail obligatoire](/settings/general.md) ;
* [gérer les utilisateurs](/users/user-management.md) ;
* [gérer l'affichage selon le type d'utilisateur](/settings/display.md).

### Un portail personnalisable

Le portail de données peut être personnalisé aux couleurs de votre organisme \(charte graphique, logo, menu affichés, authentification, etc.\). Ci-dessous quelques-unes de nos réalisations :

* GéoLorient : [http://geocatalogue.lorient-agglo.bzh/](http://geocatalogue.lorient-agglo.bzh/)
* Syndicat Mixte d’Aménagement de la Vallée de la Durance \(privé\) [http://smavd.isogeo.net](http://smavd.isogeo.net)
* Le portail de démonstration \(parfois en travaux\) : [http://demo.isogeo.net](http://demo.isogeo.net)

#### Interface multi-supports

L'interface du portail est responsive design pour s'adapter aux différents formats des supports de consultation \(ordinateur, smartphone, tablette...\).

![](/assets/front_misc_responsive_smartphone_homepage.jpg)

### Un champ fonctionnel large, complet et cohérént

Beaucoup d’autres fonctionnalités viennent compléter l'expérience utilisateur :

* export des métadonnées au format PDF ;
* des statistiques pour le reporting de l'administrateur : généralistes \(Google Analytics\) et spécifiques \(vues, ressources, recherches, etc.\) ;
* un référencement optimisé pour les moteurs de recherche \(SEO\) ;
* lien direct vers l’édition de la fiche de métadonnées pour les éditeurs Isogeo ;
* interprétation du [langage Markdown](http://help.isogeo.com/fr/features/documentation/syntax_markdown.html) disponible dans Isogeo ;
* bouton pour copier le chemin d’une donnée fichier dans le presse-papiers directement depuis la métadonnée ;
* générer un code d’intégration iFrame à partir de chaque fiche de métadonnées ;
* des liens universels basés sur l'identifiant Isogeo. Exemple : [http://demo.isogeo.net/?muid=56ed291af72f46dc9835fc9ae29fe938](http://demo.isogeo.net/?muid=56ed291af72f46dc9835fc9ae29fe938)



