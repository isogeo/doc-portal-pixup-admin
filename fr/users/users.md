---
description: Administrer les utilisateurs du portail Isogeo
---
# Utilisateurs

Ce menu permet de créer, modifier et supprimer les utilisateurs du portail.

## Utilisateurs existants {#list-users}

Ce menu permet d'afficher la liste de tous les utilisateurs. La recherche fonctionne sur tous les champs du tableau (Nom, Prénom, Email et Droit), un système de pagination a également été implémenté. Vous pouvez éditer un utilisateur en le sélectionnant mais aussi supprimer un ou plusieurs utilisateurs.

!["Menu Utilisateurs existants"](/assets/back_list_user.png)

## Edition d'un utilisateur {editing-user}

Pour créer un utilisateur, il suffit de cliquer sur `Édition d'un utilisateur` dans le menu d'accès. Pour éditer un utilisateur existant, il suffit de la sélectionner dans le menu précédent.

Dans les deux cas, vous pourrez utiliser l'éditeur personnalisé dont les champs à renseigner sont les suivants (en **gras** ceux qui sont obligatoires) :

* **Droit** : [Niveau de droit](#rights)
  * Super Admin
  * Admin rédacteur
  * Utilisateur authentifié
  * Utilisateur avec privilèges
* **Nom** : Nom de l'utilisateur
* **Prénom** Prénom de l'utilisateur
* **Email**: Mail de l'utilisateur
* Téléphone : Téléphone de l'utilisateur
* Fonction : Fonction de l'utilisateur
* Service : Service auquel appartient l'utilisateur
* **Mot de passe** : minimum 12 caractères de 4 types différents (parmi la liste ci-dessous)
  * Au moins une majuscule (A, B, C...) 
  * Au moins une minuscule (a, b, c...)
  * Au moins un chiffre (1, 2 , 3...)
  * Au moins un caractère spécial (!, $, %, &....)
  * Au moins une parenthèse ([,],{,},(,),<,>)
* **Confirmation du mot de passe** : Confirmer le mot de passe
* Remarques : Remarques associées à l'utilisateur
* Utilisateur Isogeo : L'utilisateur a t'il accès à la plateforme d'administration et d'édition des métadonnées (app.isogeo.com) ?
* Utilisateur actif : L'utilisateur est-il actif sur le portail ?

!["Editer un utilisateur"](/assets/back_edit_user.png)

## Niveaux de droits {#rights}

Isogeo distingue plusieurs profils utilisateurs :

* Super Admin

Le super Admin peut administrer et configurer tout le portail Isogeo via l'[interface d'administration](http://demo.isogeo.net/admin/menu.php?menu_item=dashboard). Il a également tous les droits de consultation de façon à pouvoir vérifier toutes ses modifications.

* Admin rédacteur

L' admin rédacteur a lui aussi accès à l'[interface d'administration](http://demo.isogeo.net/admin/menu.php?menu_item=dashboard). Cependant il ne peut modifier que le contenu du portail \(actualités, menus...\). 

* Utilisateur privilégié

L'utilisateur privilégié est un utilisateur particulier qui peut jongler entre le portail Isogeo et l'[application Isogeo](https://app.isogeo.com/). En effet, sur une fiche de métadonnée, il dispose du lien vers la fiche de métadonnées "mère" dans l'application Isogeo. S'il possède les droits de modification, il peut donc éditer directement la fiche de métadonnées puis consulter ses modifications dans le portail. En revanche cet utilisateur n'a pas accès à l'interface d'administration.

* Utilisateur authentifié

L' utilisateur authentifié peut utiliser la plupart des fonctionnalités du portail. Il peut consulter les fiches de métadonnées, les actualités, créer des listes, noter les fiches etc...

## Matrice des droits utilisateurs {#matrice}

Voici ci-dessous les fonctionnalités ouvertes en fonction du type d'utilisateur.

> ATTENTION : Il s'agit des fonctionnalités par défaut. L'affichage de certaines informations et certaines fonctionnalités sont modifiables par le super administrateur dans les [paramètres d'affichage selon le niveau de droits](/fr/settings/display/user-display). 

| Fonctionnalités                                                                   | Super Admin | Admin rédacteur | Utilisateur privilégié | Utilisateur authentifié |
|-----------------------------------------------------------------------------------|:-----------:|:---------------:|:----------------------:|:-----------------------:|
| Effectuer une recherche                                                           |X|X|X|X|
| Afficher une métadonnées                                                          |X|X|X|X|
| Télécharger une ressource                                                         |X|X|X|X|
| Créer une liste                                                                   |X|X|X|X|
| Sauvegarder une fiche dans une liste                                              |X|X|X|X|
| Commenter une fiche (onglet Discussion)                                           |X|X|X|X|
| Lire les actualités                                                               |X|X|X|X|
| Contacter les administrateurs                                                     |X|X|X|X|
| Gérer son compte (Listes, paramètres, licences, mot de passe)                     |X|X|X|X|
| Accéder au lien vers la fiche dans app.isogeo de façon à l'éditer si autorisation |X|X|X||
| Partager une fiche en iframe                                                      |X|X|X||
| Copier le chemin                                                                  |X|X|X||
| Accéder à l'interface d'administration                                            |X|X|||
| Visualiser les statistiques du portail (dashboard)                                |X|X|||
| Configurer les actualités (ajout, édition, suppression)                           |X|X|||
| Configurer les médias (images, fichiers)                                          |X|X|||
| Gérer les pages et iFrames (ajout, édition, suppression)                          |X|X|||
| Configurer les pages d'accueil marketing et métiers                               |X||||
| Configurer les menus                                                              |X||||
| Gérer les Dataviz                                                                 |X||||
| Gérer les messages et les commentaires                                            |X||||
| Gérer les paramètres (généraux, affichage selon utilisateur, recherche...)        |X||||
| Gérer le cache des services                                                       |X||||
| Gérer les utilisateurs (Ajout, droits, suppression)                               |X||||