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
* les polygones doivent être dessinés dans le sens anti-horaire \(sens inverse des aiguilles d'une montre\), selon la règle dite [_Left-Hand-Rule_](http://www.scalefocus.com/blog/using-spatial-data-in-sql-server-the-left-hand-rule/) \(voir aussi [la doc Microsoft](https://docs.microsoft.com/en-us/sql/relational-databases/spatial/spatial-data-types-overview)\).
* l'emprise spatiale \(bbox\) doit être incluse par objet \(voir [http://geojson.org/geojson-spec.html\#bounding-boxes](http://geojson.org/geojson-spec.html#bounding-boxes)\)

Pour créer le fichier correctement, il est recommandé de passer par un outil dédié :

* QGIS \(voir ci-dessous\) ;
* [geojson.io](http://geojson.io/).

##### Création depuis QGIS

1. Ouvrir le fichier d'emprises ou créer un nouveau fichier vectoriel ;
2. Modifier la structure attributaire pour ne garder que `id` et `name` ;
3. Dessiner les emprises dans le sens anti-horaire ;
4. Sauvegarder les 

![](/assets/back_search_bbox_qgis_howtosave.png)

![](/assets/back_search_bbox_qgis_structure.png)

##### Exemple de fichier _recherche\_geo\_emprises.geojson_

```js
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {
        "id": 1,
        "name": "PBW Events"
      },
      "bbox": [
        2.174567705830178,
        48.61840838516793,
        2.579169415881337,
        48.94676296444957
      ],
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              2.2397467047138,
              48.934465040131904
            ],
            [
              2.31230445818802,
              48.94676296444957
            ],
            [
              2.31230445818802,
              48.94676296444957
            ],
            [
              2.395930343548137,
              48.943073587154274
            ],
            [
              2.574250246154271,
              48.86190728665768
            ],
            [
              2.579169415881337,
              48.66391070514329
            ],
            [
              2.373794079776342,
              48.61840838516793
            ],
            [
              2.174567705830178,
              48.62947651705383
            ],
            [
              2.2397467047138,
              48.934465040131904
            ]
          ]
        ]
      }
    },
    {
      "type": "Feature",
      "properties": {
        "id": 2,
        "name": "La Réunion - AH"
      },
      "bbox": [
        54.18915481038568,
        -22.581765019733755,
        57.036733431104786,
        -19.89249980699394
      ],
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              54.56883195981489,
              -20.35594487016747
            ],
            [
              55.93566969776006,
              -19.89249980699394
            ],
            [
              56.61908856673264,
              -20.747008661495475
            ],
            [
              57.036733431104786,
              -21.843621587104487
            ],
            [
              56.049572842588816,
              -22.581765019733755
            ],
            [
              54.75867053452949,
              -22.441466473313262
            ],
            [
              54.18915481038568,
              -21.49077159840838
            ],
            [
              54.56883195981489,
              -20.35594487016747
            ]
          ]
        ]
      }
    },
    {
      "type": "Feature",
      "properties": {
        "id": 3,
        "name": "La Réunion - H"
      },
      "bbox": [
        52.100930488525,
        -24.046151682954022,
        58.28966802422118,
        -19.033354591216522
      ],
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              53.5057359414131,
              -19.140995564363013
            ],
            [
              55.442089403502074,
              -19.033354591216522
            ],
            [
              56.5431531368468,
              -19.570854704343983
            ],
            [
              57.49234601041983,
              -21.137063973947583
            ],
            [
              58.28966802422118,
              -23.385690639372825
            ],
            [
              55.21428311384455,
              -24.046151682954022
            ],
            [
              52.89825250232636,
              -23.490195777493803
            ],
            [
              52.100930488525,
              -21.526095378081454
            ],
            [
              53.5057359414131,
              -19.140995564363013
            ]
          ]
        ]
      }
    },
    {
      "type": "Feature",
      "properties": {
        "id": 4,
        "name": "Brésil - AH"
      },
      "bbox": [
        -76.00213972889141,
        -35.82350598876392,
        -30.137140077842496,
        6.976857147967661
      ],
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              -51.24718958610673,
              6.675268846027083
            ],
            [
              -41.67932542049057,
              5.920502837764745
            ],
            [
              -30.137140077842496,
              -2.269365701452029
            ],
            [
              -30.896494376700936,
              -5.904381844311442
            ],
            [
              -33.630169852591266,
              -12.94132842797136
            ],
            [
              -35.14887845030811,
              -24.703233145000826
            ],
            [
              -41.527454560718894,
              -34.0809479979276
            ],
            [
              -52.46215646428021,
              -35.82350598876392
            ],
            [
              -59.14447429423435,
              -34.0809479979276
            ],
            [
              -58.23324913560425,
              -28.903968767621908
            ],
            [
              -60.05569945286447,
              -23.315974699716378
            ],
            [
              -59.9038285930928,
              -20.07091034670052
            ],
            [
              -64.45995438624335,
              -16.02881457234864
            ],
            [
              -72.9647225334577,
              -12.4968972838023
            ],
            [
              -76.00213972889141,
              -6.055426253579809
            ],
            [
              -72.81285167368603,
              0.463711121062637
            ],
            [
              -69.01608017939388,
              4.710783855317874
            ],
            [
              -61.42253719080964,
              6.976857147967661
            ],
            [
              -51.24718958610673,
              6.675268846027083
            ]
          ]
        ]
      }
    },
    {
      "type": "Feature",
      "properties": {
        "id": 5,
        "name": "Île de Pâques - AH"
      },
      "bbox": [
        -109.73882743786092,
        -27.513409578195237,
        -108.78963456428788,
        -26.81671013907495
      ],
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              -109.35677730624778,
              -26.81671013907495
            ],
            [
              -108.95099735279531,
              -26.882342236753193
            ],
            [
              -108.78963456428788,
              -27.076896857399056
            ],
            [
              -108.87031595854158,
              -27.319615834961567
            ],
            [
              -109.17643066026889,
              -27.513409578195237
            ],
            [
              -109.50627518383553,
              -27.500781227059445
            ],
            [
              -109.73882743786092,
              -27.334372953869458
            ],
            [
              -109.67475691889474,
              -26.977546841569673
            ],
            [
              -109.56085377406596,
              -26.850589522530655
            ],
            [
              -109.35677730624778,
              -26.81671013907495
            ]
          ]
        ]
      }
    },
    {
      "type": "Feature",
      "properties": {
        "id": 6,
        "name": "Île de Pâques - H"
      },
      "bbox": [
        -109.56559973843383,
        -27.2922045477882,
        -109.10998715911877,
        -26.99657811375575
      ],
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              -109.42322080739785,
              -26.99657811375575
            ],
            [
              -109.10998715911877,
              -27.089573509380195
            ],
            [
              -109.15744680279741,
              -27.233141870958043
            ],
            [
              -109.39474502119067,
              -27.2922045477882
            ],
            [
              -109.56559973843383,
              -27.233141870958043
            ],
            [
              -109.56559973843383,
              -27.072670988055336
            ],
            [
              -109.42322080739785,
              -26.99657811375575
            ]
          ]
        ]
      }
    }
  ]
}
```



