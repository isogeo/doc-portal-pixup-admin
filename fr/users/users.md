---
description: Administrer les utilisateurs du portail Isogeo
---
# Utilisateurs

Ce menu permet de créer, modifier et supprimer les utilisateurs du portail.

## Utilisateurs existants {#list-users}

Ce menu permet d'afficher la liste de tous les utilisateurs. La recherche fonctionne sur tous les champs du tableau (Nom, Prénom, Email et Droit). Vous pouvez éditer un utilisateur en le sélectionnant mais aussi supprimer un ou plusieurs utilisateurs. Vous pouvez filtrer sur les utilisateurs d'un groupe en particulier ou sélectionner plusieurs utilisateurs pour les affecter par lot à un ou plusieurs groupes.

!["Menu Utilisateurs existants"](/assets/back_list_user.png)

## Edition d'un utilisateur {#editing-user}

Pour créer un utilisateur, il suffit de cliquer sur `Édition d'un utilisateur` dans le menu d'accès. Pour éditer un utilisateur existant, il suffit de le sélectionner dans le menu précédent.

Dans les deux cas, vous pourrez utiliser l'éditeur personnalisé dont les champs à renseigner sont les suivants (en **gras** ceux qui sont obligatoires) :

* **Groupe** : [Groupe de droit](/groups/groups.md#group-display)
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
* Utilisateur Isogeo : L'utilisateur a-t-il accès à la plateforme d'administration et d'édition des métadonnées (app.isogeo.com) ?
* Utilisateur actif : L'utilisateur est-il actif sur le portail ?

!["Editer un utilisateur"](/assets/back_edit_user.png)

## Paramétrage par défaut des droits des groupes utilisateurs {#matrice}

Voici ci-dessous les fonctionnalités ouvertes en fonction du type d'utilisateur.

> ATTENTION : Il s'agit des fonctionnalités par défaut. L'affichage de certaines informations et certaines fonctionnalités sont modifiables par le super administrateur dans les [paramètres d'affichage des différents groupes](/groups/groups.md#group-display).

| Fonctionnalités                                                                   | Super Admin | Utilisateur authentifié | Utilisateur public |
|-----------------------------------------------------------------------------------|:-----------:|:----------------------:|:-----------------------:|
| Effectuer une recherche                                                           |X|X|X|
| Afficher une métadonnée                                                           |X|X|X|
| Télécharger une ressource                                                         |X|X|X|
| Créer une liste                                                                   |X|X|X|
| Sauvegarder une fiche dans une liste                                              |X|X|X|
| Commenter une fiche (onglet Discussion)                                           |X|X|X|
| Contacter les administrateurs                                                     |X|X|X|
| Gérer son compte (Listes, paramètres, licences, mot de passe)                     |X|X|X|
| Accéder au lien vers la fiche dans app.isogeo de façon à l'éditer si autorisation |X|X||
| Partager une fiche en iframe                                                      |X|X||
| Copier le chemin                                                                  |X|X||
| Accéder à l'interface d'administration                                            |X|||
| Visualiser les statistiques du portail (dashboard)                                |X|||
| Configurer les actualités (ajout, édition, suppression)                           |X|||
| Configurer les médias (images, fichiers)                                          |X|||
| Gérer les pages et iFrames (ajout, édition, suppression)                          |X|||
| Configurer le page d'accueil                                                      |X|||
| Configurer les menus                                                              |X|||
| Gérer les Dataviz                                                                 |X|||
| Gérer les messages et les commentaires                                            |X|||
| Gérer les paramètres (généraux, affichage selon utilisateur, recherche...)        |X|||
| Gérer les utilisateurs (Ajout, suppression)                                       |X|||
| Gérer les groupes (Ajout, droits, suppression)                                    |X|||
