---
description: Gérer les iFrames intégrés au portail Isogeo
---
# iFrames

Ce menu permet de gérer les pages que vous souhaitez intégrer en iFrame à votre portail. Vous pouvez donc créer, modifier, supprimer des iFrames.

## iFrames existantes {#list-iframes}

Ce menu permet d'afficher la liste de toutes les iFrames. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer une iFrame ou les supprimer par lot.

!["Menu iFrames existantes"](/assets/back_list_iframe.png)

## Edition d'une iFrame {#editing-iframe}

Pour créer une iFrame, il suffit de cliquer sur `Édition d'une iFrame` dans le menu d'accès. Pour éditer une iFrame existante, il suffit de la sélectionner dans le menu précédent.
Dans les deux cas, vous pourrez utiliser l'éditeur personnalisé dont les champs à renseigner sont les suivants (en **gras** ceux qui sont obligatoires) :

__Onglet Infos principales__
* **Titre** : Nom de l'iFrame
* **URL** : URL de la page à intégrer

__Onglet Méta-balises__
* **Titre** : Nom de l'iFrame
* Keywords : Mots-clés pour le référencement de la page
* Description : Mini-résumé descriptif de l'iFrame

__Onglet Publication__
* Rubrique : Sélectionner le menu du site où vous souhaitez intégrer l'iFrame.
* Groupes autorisés : sélectionner les groupes d'utilisateurs autorisés à consulter l'iFrame.
* Cette iFrame est un brouillon : Si non, l'iFrame est publié pour les groupes autorisés.

!["Editer une iFrame"](/assets/back_edit_iframe.png)

## Résultat sur le front-office {#result}

Dans cet exemple, nous avons voulu intégrer en iFrame notre widget Web App Builder de démonstration. Voici le résultat :

!["Intégration d'une page en iFrame - côté front"](/assets/front_iframe.png)