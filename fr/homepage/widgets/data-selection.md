---
description: Gérer le widget de sélection de données géographiques de la page d'accueil du portail Isogeo
---
# Sélection de données

Ce widget permet de sélectionner les données que vous souhaitez mettre en avant depuis la page d'accueil du site. Vous pouvez personnaliser cette sélection dans les menus suivants.

## Données sélectionnées {#list-selections}

Ce menu permet d'afficher la liste de toutes les données sélectionnées. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer une sélection ou en supprimer une ou plusieurs si besoin. 

!["Menu Sélections existantes"](/assets/back_list_selection.png)

## Ajout d'une donnée {#editing-selection}

Pour créer une sélection, il suffit de cliquer sur `Ajout d'une donnée` dans le menu d'accès. Pour éditer une sélection de donnée existante, il suffit de la sélectionner dans le menu précédent.

Pour sélectionner une donnée, il faut préalablement récupérer son identifiant dans l'URL de la fiche de métadonnées sur le portail.

!["Récupérer l'ID de la métadonnée"](/assets/find_md_id_portal.png)

Un fois l'ID récupéré, il suffit de cliquer sur mettre à jour pour générer automatiquement la fiche.

## Résultat sur le front-office {#result}

### Widget dans la page d'accueil {#front-widget-selection}

Les sélections sont présentées dans un widget de type "Slider". En cliquant sur le titre, l'utilisateur accède directement à la fiche concernée dans le portail. Vous pouvez faire défiler les données sélectionnées en maintenant et relachant le clic gauche souris.  

!["Widget sélection de données - côté front"](/assets/front_widget_selection.png)

# Sélection de données Dawizz

Lorsque l'API Dawizz est [activée](/settings/general.md#api), le widget de sélection de données précédent est remplacé automatiquement par celui-ci.

Ce widget permet de sélectionner les données du catalogue que vous souhaitez mettre en avant depuis la page d'accueil du site. Vous pouvez personnaliser cette sélection dans les menus suivants.

## Sélections existantes {#list-selections}

Ce menu permet d'afficher la liste de toutes les données sélectionnées. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer une sélection ou en supprimer une ou plusieurs si besoin. 

!["Menu Sélections existantes"](/assets/back_list_selection_dawizz.png)

## Edition d'une sélection {#editing-selection}

Pour créer une sélection, il suffit de cliquer sur `Ajout d'une sélection` dans le menu d'accès. Pour éditer une sélection existante, il suffit de la sélectionner dans le menu précédent.

Pour sélectionner une donnée, il faut préalablement récupérer son identifiant Dawizz. Pour information, l'ID correspond au nom de la donnée et se trouve dans l'url d'une métadonnée sur app.dawizz.fr.

!["Récupérer l'ID de la métadonnée"](/assets/find_md_id_app_dawizz.png)

Un fois l'ID récupéré, il suffit de cliquer sur mettre à jour pour générer automatiquement la fiche.

![Fiche générée](/assets/back_edit_selection_dawizz.png)

## Résultat sur le front-office {#result}

### Widget dans la page d'accueil {#front-widget-selection}

Les sélections sont présentées dans un widget de type "Slider". En cliquant sur le titre, l'utilisateur accède directement à la fiche concernée dans le portail. Vous pouvez faire défiler les données sélectionnées en maintenant et relachant le clic gauche souris.

!["Widget sélection de données - côté front"](/assets/front_widget_selection_dawizz.png)