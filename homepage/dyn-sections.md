# Pavés dynamiques

Les pavés dynamiques permettent d'afficher, sur la page d'accueil, des listes de données selon différents critères définis par l'administrateur du portail. Le but est d'une part de mettre facilement en avant l'actualité des données et d'autre part de garantir une certaine fraîcheur au portail sans que l'administrateur ne soit contraint de créer ou mettre à jour des contenus régulièrement.

## Fonctionnement

Les pavés listent des données selon des critères liés à l'API Isogeo \(dates de création et dernière modification des données et métadonnées par exemple\) ou propres au portail \(évaluations par exemple\). Chaque métadonnée est présentée sous forme d'un pavé.

!["Administrer les blocs dynamiques en page d'accueil"](/assets/back_homepage_dynamic_sections.png)

## Réglages

Le portail permet de configurer jusqu'à 3 blocs. Chaque bloc peut être masqué ou affiché sur 1 ou 2 colonnes.

### Colonne

Chaque colonne est configurable :

* **Titre de la colonne**. Il est recomandé de limiter à des mots de 25 caractères continus pour éviter les problèmes de mise en page.

* **Variable de contenu**. Valeurs possibles :

  * données récemment modifiées - API Isogeo
  * métadonnées récemment modifiées  - API Isogeo
  * données récemment créées - API Isogeo
  * métadonnées récemment créées  - API Isogeo
  * données sélectionnées - Portail
  * données les plus commentées - Portail
  * données les mieux notées - Portail
  * données les moins consultées - Portail

* **Nombre de pavés par colonne**. Il est recommandé de définir le même nombre entre 2 colonnes d'un même bloc. Valeurs possibles :

  * 2
  * 4
  * 6
  * 8

#### Pavé

Chaque pavé contient 1 métadonnée :

* Titre \(obligatoire\).
* les 300 premiers caractères du résumé  : il est possible de définir si les balises markdown sont interprétéés ou pas.
* Propriétaire de la métadonnée \(facultatif\) ;
* Echelle \(facultatif\).
* Type \(facultatif\).

Les paramètres facultatifs dépendent du type d'utilisateur et sont donc configurables dans la rubique [Affichage  
](/settings/display.md).

