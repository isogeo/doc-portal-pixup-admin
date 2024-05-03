---
description: Ecrire un article présentant une actualité dans le portail Isogeo
---
# Actualités

Ce menu permet de rédiger des articles autour du SIG. Vous pouvez créer, modifier ou supprimer des articles et les ranger par catégorie.

## Articles existants {#list-news}

On retrouve ici la liste de tous les articles rédigés. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer un article ou en supprimer un ou plusieurs si besoin.

!["Menu articles existants"](/assets/back_list_article.png)

## Edition d'un article {#editing-news}

Pour créer un article, il suffit de cliquer sur `Édition d'un article` dans le menu d'accès. Pour éditer un article existant, il suffit de le sélectionner dans le menu précédent.

!["Editer un article"](/assets/back_edit_article.png)

Le menu d'édition d'un article présente donc 4 onglets.

### Infos principales {#main-informations}

Cet onglet permet de compléter les informations contenues dans l'étiquette de présentation de l'article dans la page de [présentation des articles](#front-news-page).

* Visuel : *Insérer une image avec le [gestionnaire de fichiers](/medias/filesmanager.md) intégré au portail.*
* Titre : *Nouveau module de Dataviz !*
* Date : *01/10/2019*
* Résumé : *Les données sont une chose, leur représentation en est une autre. Pour dépasser les limites d'un affichage purement textuel, nous avons préparé plusieurs exemples de visualisations graphiques de vos données géographiques.*
* Catégorie : *Général*

!["Exemple d'étiquette de présentation d'une actualité"](/assets/front_news_tag.png)

### Méta-balises {#meta-tags}

Les méta-balises permettent d'améliorer le référencement dans les moteurs de recherche pour les portails publics. Les champs obligatoires sont en **gras**.

* **Title** : Le champ *title* est celui qui apparaît dans la barre de titre ou d’onglet du navigateur.
  * Exemple : *Nouveau module de Dataviz !*
* Keywords : Les mots-clés doivent étre séparés par des virgules.
  * Exemple : *data, dataviz, données géographiques, isogeo, portail, catalogue*
* Description : Le champ *description* est celui qui apparaît dans la page de résultats de recherche des moteurs de recherche.
  * Exemple : *Cette page présente la nouvelle fonctionnalité de consultation du catalogue de données sous forme de data-visualisation du portail Isogeo.*

### Corps de l'article {#body}

Le corps de l'article permet de rédiger le contenu de l'actualité à l'aide de [l'éditeur WYSIWYG intégré](/appendices/editorwysiwyg.md).

!["Exemple de contenu dans le back-office"](/assets/back_news_dataviz.png)

On retrouve ce contenu sur la page dédiée à l'actualité accompagné des informations principales saisies précédemment (cf. Exemple ci-dessous).

!["Exemple d'actualité dans le front-office"](/assets/front_news_dataviz.png)

### Publication {#publishing}

Cet onglet permet de gérer la publication de l'actualité.

* Cet article est un brouillon : Si non, l'article est publié sur la page des actualités pour les groupes autorisés.
* Groupes autorisés : sélectionner les groupes d'utilisateurs autorisés à consulter l'actualité.
* Date de début de publication : Sélectionner une date à partir de laquelle l'actualité sera visible sur le portail
* Date de fin  de publication : Sélectionner une date à partir de laquelle l'actualité ne sera plus visible sur le portail.
* Afficher sur l'accueil : Si oui, l'actualité est affichée dans le widget de sélection sur la page d'accueil. (cf. [Widget sur la page d'accueil](#widget-last-news))

## Gestion des catégories {#categories}

### Liste des catégories existantes {#list-categories}

Ce menu permet de créer des catégories pour ranger vos articles. Par défaut, la catégorie `Général` est créée et affectée à tous vos articles.

### Édition d'une catégorie {#editing-categories}

Pour créer une nouvelle catégorie, cliquer sur `Nouvelle saisie` puis éditer le nom avant d'enregistrer.
Pour éditer une catégorie existante, cliquer sur la catégorie dans la liste précédente puis éditer le nom avant d'enregistrer.

> NB : la catégorie `Général` ne peut être éditée ou supprimée.

!["Gestion des catégories"](/assets/back_edit_category.png)

### Affectation d'une catégorie à un article {#affect-categories}

Dans l'éditeur de contenu des articles, onglet *Informations principales*, vous pouvez choisir la catégorie concernée.

## Résultat sur le front-office {#result-front}

### Widget dans la page d'accueil {#widget-last-news}

Un widget de type "Slider" est automatiquement généré sur la page d'accueil contenant les actualités publiées. Vous pouvez faire défiler les actualités en maintenant et relachant le clic gauche souris.  

!["Widget dernières actualités - côté front"](/assets/front_widget_article.png)

### Page de présentation des actualités {#front-news-page}

Une page regroupe l'ensemble des actualités. Par défaut, le portail est paramétré pour que cette page soit accessible depuis le menu du site "Actualités'", dans la page d'accueil. Depuis cette page, vous pouvez donc lire les actualités d'un simple clic !

!["Page de présentation des actualités - côté front"](/assets/front_article.png)