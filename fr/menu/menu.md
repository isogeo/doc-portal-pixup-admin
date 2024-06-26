---
description: Gérer les menus du portail Isogeo
---
# Menus du site

Ce menu permet de gérer les menus de ce portail. Vous pouvez ajouter, modifier des menus et gérer leur ordre d'affichage.

## Eléments existants {#list-elements}

Ce menu permet d'afficher la liste de tous les menus. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer un menu ou en supprimer un ou plusieurs si besoin. 

!["Menu Eléments existants"](/assets/back_list_menu.png)

## Edition d'un menu {#editing-element}

Pour créer un menu, il suffit de cliquer sur `Édition d'un élément` dans le menu d'accès. Pour éditer un menu existant, il suffit de le sélectionner dans le menu précédent.
L'éditeur permet de modifier les champs suivants (ceux en **gras** étant obligatoires):

* **Titre**
* **Type d'entrée**
    * Lien vers accueil du site : soit la [page contenant les différents Widgets](/homepage/titles.md)
    * Lien vers la page "Actualités" : soit la [page de présentation des actualités](/homepage/widgets/news.md)
    * Lien vers la page "Contact" : soit la [page de contact](/messages-recus/contacts.md)
    * Lien vers la page "Catalogue" : soit la [page de recherche dans le catalogue de données](/introduction.md)
    * Lien vers la page "Dataviz" : soit la [page de consultation des Dataviz](/dataviz/dataviz.md)
    * Lien vers une page : soit les pages restantes du site parmi la [liste des pages existantes](/pages-iframes/pages.md)
    * Lien vers une actualité : soit une actualité parmi la liste des [actualités existantes](/homepage/widgets/news.md)
    * Saisie d'une url directe : soit une URL externe au portail
        * **Url** : soit l'url en question
        * Fenêtrage : choisir si le lien doit être ouvert dans une nouvelle fenêtre ou dans la fenêtre courante
    * Lien vers une iFrame : soit une iFrame parmi la [liste des iFrames existantes](/pages-iframes/iframes.md)
* Groupes autorisés : sélectionner les groupes d'utilisateurs autorisés à consulter le menu.
* Cet élément de menu est un brouillon : Si non, le menu est publié pour les groupes autorisés.

!["Editer un menu"](/assets/back_edit_menu.png)

## Gérer l'ordre {#order}

Ce menu permet de modifier simplement l'ordre d'affichage des menus.
En effet, il suffit de sélectionner un menu et de le glisser déposer avant ou après les autres.
N'oubliez pas ensuite d'enregistrer en utilisant le bouton <i class="ti-save"></i> en bas à droite de la page.

> NB : L'ensemble des menus sont affichés dans ce menu même si ces derniers sont dépubliés. Les menus dépubliés sont affichés en rouge.

!["Changer l'ordre d'affichage des menus"](/assets/back_order_menu.png)

## Résultat sur le front-office {#result}

Les menus sont accessibles en permanence lors de la navigation sur le portail car ils sont ajoutés à l'en-tête du site.

!["Menu du site - côté front"](/assets/front_menu.png)