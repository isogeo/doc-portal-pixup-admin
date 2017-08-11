## Recherche par emprises personnalisées

### Fonctionnement

L’administrateur du portail peut établir une liste d'emprises "pertinentes" au regard du patrimoine mis en valeur et des utilisateurs. Elles présentent l’avantage d’être des zones géographiques indépendantes des limites administratives \(une zone de projet par exemple\) ou adresse \(remontée par le géocodeur\).

Du côté de l’utilisateur, une liste déroulante apparaît à côté de la zone de saisie "Localisation" dans la zone de recherche.

### Options

#### Activer / désactiver

Se rendre dans la section "Médias / Gestionnaire de fichiers" ;

1. Dans le répertoire "files/recherche\_geo", enregistrer le fichier des emprises \(voir spécifications plus bas\) ;
2. Se rendre dans la section "Paramètres site / Configuration" ;
3. Au paragraphe "Fichier de recherche Géo", vérifier que les emprises sont correctement listées ;
4. Activer/désactiver dans la liste déroulante.

Pour supprimer la recherche des emprises, il faut depuis le B.O. :

* supprimer le fichier depuis la section "Médias / Gestionnaire de fichiers"
* vérifier que cette suppression a bien été prise en compte en se rendant dans la section "Paramètres site / Configuration". Cette dernière étape est impérative.

#### Ajouter le fichier d’emprises {#docs-internal-guid-124f9e3a-d1f4-3bf4-8332-97132986e7cf}

Pour permettre la recherche par emprise, un fichier doit être créé et déposé par l’admnistrateur. Il doit respecter certaines caractéristiques :

* format GeoJSON \([http://geojson.org](http://geojson.org)\) ;
* le fichier doit se nommer “recherche\_geo\_emprises.geojson”
* 2 attributs obligatoires : id et name. Exemple : `"properties":{"id":5,"name":"Bassin d'Arcachon"}`
* projection WGS84 \(EPSG 4326\). Exemple : `"crs":{"type":"name","properties":{"name":"urn:ogc:def:crs:OGC:1.3:CRS84"}}`,
* précision des coordonnées =&lt; 3 ;
* encodage UTF-8 ;
* géométries de type polygone ;
* les polygones doivent être dessinés dans le sens anti-horaire \(sens inverse des aiguilles d'une montre\), selon la règle diteLeft-Hand-Rule.
* l'emprise spatiale \(bbox\) doit être incluse par objet \(voir [http://geojson.org/geojson-spec.html\#bounding-boxes](http://geojson.org/geojson-spec.html#bounding-boxes)\)

Exemple de création depuis QGIS :

![](/assets/back_search_bbox_qgis_howtosave.png)

![](/assets/back_search_bbox_qgis_structure.png)

