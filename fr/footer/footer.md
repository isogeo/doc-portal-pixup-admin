---
description: Gérer le pied de page portail Isogeo
---
# Pied de page

Ce menu permet de gérer le pied de page du portail. Vous pouvez ajouter, modifier des éléments du pied de page et gérer leur ordre d'affichage.

Pour information, le pied de page comporte par défaut le plan du site qui est généré automatiquement et un lien vers le site officiel d'Isogeo. Il contient également les liens vers les réseaux sociaux renseignés dans les [paramètres généraux](/settings/general.md#social_network). 

## Eléments existants {#list-elements}

Ce menu permet d'afficher la liste de tous les éléments du pied de page. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer un élément ou en supprimer un ou plusieurs si besoin. 

!["Menu Eléments existants"](/assets/back_list_footer.png)

## Edition d'un élément {#editing-element}

Pour ajouter un élément au pied de page, il suffit de cliquer sur `Édition d'un élément` dans le menu d'accès. Pour éditer un élément existant, il suffit de le sélectionner dans le menu précédent.
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
* Groupes autorisés : sélectionner les groupes d'utilisateurs autorisés à consulter l'élément du pied de page.
* Cet élément est un brouillon : Si non, l'élément est publié pour les groupes autorisés.

!["Editer un élément"](/assets/back_edit_footer.png)

## Gérer l'ordre {#order}

Ce menu permet de modifier simplement l'ordre d'affichage des éléments du pied de page. En effet, il suffit de sélectionner un élément et de le glisser déposer avant ou après les autres.
N'oubliez pas ensuite d'enregistrer en utilisant le bouton <i class="ti-save"></i> en bas à droite de la page.

> NB : L'ensemble des éléments du pied de page sont affichés dans ce menu même si ces derniers sont dépubliés. Les éléments dépubliés sont affichés en rouge.

!["Changer l'ordre d'affichage des éléments"](/assets/back_order_footer.png)

## Résultat sur le front-office {#result}

Les éléments publiés sont accessibles en permanence lors de la navigation sur le portail car ils sont ajoutés au pied de page du site.

!["Pied de page - côté front"](/assets/front_footer.png)