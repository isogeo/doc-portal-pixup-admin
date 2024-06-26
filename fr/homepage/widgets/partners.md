---
description: Gérer le widget Partenaires de la page d'accueil du portail Isogeo
---
# Partenaires

Ce widget permet de présenter les différents partenaires du SIG au sein de votre structure. Vous pouvez créer, modifier des articles pour présenter ces différents partenaires et gérer leur ordre d'affichage.

## Partenaires existants {#list-partners}

Ce menu permet d'afficher la liste de tous les partenaires. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer un partenaire ou en supprimer un ou plusieurs si besoin. 

!["Menu partenaires existants"](/assets/back_list_partner.png)

## Edition d'un partenaire {#editing-partners}

Pour créer un partenaire, il suffit de cliquer sur `Édition d'un partenaire` dans le menu d'accès. Pour éditer un partenaire existant, il suffit de le sélectionner dans le menu précédent.

!["Editer un partenaire"](/assets/back_edit_partner.png)

Le menu d'édition d'un partenaire présente donc 4 onglets.

### Méta-balises {#meta-tags}

Les méta-balises permettent d'améliorer le référencement dans les moteurs de recherche pour les portails publics. Les champs obligatoires sont en **gras**.

* **Title** : Le champ *title* est celui qui apparaît dans la barre de titre ou d’onglet du navigateur.
* Keywords : Les mots-clés doivent étre séparés par des virgules.
* Description : Le champ *description* est celui qui apparaît dans la page de résultats de recherche des moteurs de recherche.

### Titre & visuel {#title-visual}

Cet onglet permet de gérer le titre de l'application et le visuel dans le widget Partenaires de la page d'accueil.

* **Icône** : *Insérer une image avec le [gestionnaire de fichiers](/medias/filesmanager.md) intégré au portail. N'hésitez pas à les récupérer parmi ceux proposés par Isogeo dans le répertoire logos*
  * Exemple : *Logo du partenaire*
* **Titre** : *Nom du partenaire*
  * Exemple : *Isogeo*
* Catégorie : *[Catégorie](#category) dans laquelle le partenaire sera regroupé sur le front*


### Corps de la page {#body}

Le corps de la page permet de rédiger le contenu de la page présentant le partenaire à l'aide de [l'éditeur WYSIWYG intégré](/appendices/editorwysiwyg.md). 

### Publication {#publishing}

Cet onglet permet de gérer la publication du partenaire.

* Cette fiche est un brouillon. : Si non, l'application est publiée dans le portail et accessible depuis le [widget partenaires](#widget-partners) pour les groupes autorisés.
* Groupes autorisés : sélectionner les groupes d'utilisateurs autorisés à consulter le partenaire.

## Gérer l'ordre {#order}

Ce menu permet de modifier simplement l'ordre d'affichage des partenaires. 
En effet, il suffit de sélectionner un partenaire et de le glisser déposer avant ou après les autres.
N'oubliez pas ensuite d'enregistrer en utilisant le bouton <i class="ti-save"></i> en bas à droite de la page.

> NB : Seuls les partenaires publiés sont affichés dans ce menu.

!["Changer l'ordre d'affichage des partenaires"](/assets/back_order_partner.png)

## Gestion des catégories {#category}

Vous pouvez créer plusieurs catégories pour que les partenaires soit séparés sur le widget de la page d'accueil et la page partenaires.

Pour chaque catégorie, vous pouvez indiquer son nom et les couleurs du texte et du fond qui s'afficheront sur le widget et la page partenaires.

## Résultat sur le front-office {#result}

### Widget dans la page d'accueil {#widget-partners}

!["Widget partenaire - côté front"](/assets/front_widget_partner.png)

### Page de présentation du partenaire {#front-partners}

!["Présentation d'un partenaire - côté front"](/assets/front_partner.png)