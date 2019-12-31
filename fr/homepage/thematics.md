# Thématiques des données

Cette fonctionnalité permet à l'administrateur de définir des ensembles de données estimés assez cohérents pour être présentés sous forme de thématiques.

## Fonctionnement

L'administrateur définit une recherche filtrée qu'il associe à nom de thématique. Cette thématique devient alors disponible depuis différents points du portail :

* elle est affichée sous le slogan de [la zone "Mise en avant" de la page d'accueil](/homepage/config/featured-section.md) ;
* sous forme de filtre dans l'interface de recherche du catalogue, ainsi que dans [l'interface cartographique](/settings/search-map/searchmap.md) ;
* dans les contenus éditoriaux \([Actualités](/actualites/newarticle.md) et [Pages statiques](/pages/pageseditor.md)\) ;
* dans les [zones HTML personnalisables](/homepage/config/html-area.md), sous forme de lien interne \(notamment celle de la page d'accueil\).

![&quot;Exemple de résultat du filtre par thématique dans le catalogue&quot;](/assets/front_custom_thematics_filter.png)

## Créer une thématique

1. Dans le menu `Accueil`&gt; `Sélection de données`, cliquer sur le bouton `Créer une nouvelle sélection`;
2. Dans `Intitulé`, indiquer le nom de la thématique \(celui qui s'affichera dans les différentes interfaces - obligatoire\) ;
3. Dans `Expression`, insérer les termes qui seront passés au moteur de recherche Isogeo \(facultatif\) ;
4. Dans `Catalogue Isogeo`, insérer l'identifiant du catalogue Isogeo, [trouvable dans le menu Catalogues de l'administrattion Isogeo](https://app.isogeo.com/admin/catalogs) \(facultatif\) ;
5. Cliquer sur `Enregistrer`.

![&quot;Formulaire de création d&apos;une nouvelle thématique&quot;](/assets/back_custom_thematics_new.png)

## Lier une thématique

Une fois les thématiques créées, il est donc possible de lier n'importe quel contenu HTML ou éditorial vers la recherche filtrée à laquelle elles correspondent. Par exemple via [l'éditeur WYSIWYG](/appendices/editorwysiwyg.md) :

!["Menu lien vers une thématique personnalisée"](/assets/back_custom_thematic_editor_menu.png)