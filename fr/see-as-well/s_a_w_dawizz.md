---
description: Gérer les Voir aussi Dawizz du portail Isogeo
---
# Voir aussi Dawizz

Cette section permet de gérer les **Voir aussi** Dawizz des fiches de métadonnées du portail lorsque l'API Dawizz est activée. Il s'agit d'un onglet qui présente à l'utilisateur des fiches liées à celle qu'il est en train de consulter et qui pourraient l'intéresser (cf. capture en bas de la page).

## Eléments existants {#list-elements}

Ce menu permet d'afficher la liste de tous les **Voir aussi**. Une barre de recherche (sur le nom) et un système de pagination ont été implémentés. Vous pouvez éditer un menu ou en supprimer un ou plusieurs si besoin.

!["Menu Eléments existants"](/assets/back_list_saw_dawizz.png)

## Edition d'un élément {#editing-element}

Pour créer un **Voir Aussi**, il suffit de cliquer sur `Édition d'un élément` dans le menu d'accès. Pour éditer un **Voir Aussi** existant, il suffit de le sélectionner dans le menu précédent.

L'éditeur permet de sélectionner la donnée de référence et la donnée à associer.

1. Pour récupérer l'ID Dawizz d'une fiche, il suffit de l'ouvrir dans le portail et de récupérer l'identifiant à la fin de l'URL enremplacant le "*[dot]*" par des "*.*". Par exemple : http://le64.devpixup.com/les-donnees-dawizz/Utilisateurs-ASA/ASA[dot]CASA[dot]TBUTILISATEURS donne **ASA.CASA.TBUTILISATEURS**
2. Indiquer l'identifiant de la fiche de référence et celui de la fiche cible et enregistrer. Les titres des métadonnées doivent s'afficher si les identifiants étaient corrects.

!["Editer un Voir aussi"](/assets/back_edit_saw_dawizz.png)

> Attention les **Voir aussi** ne sont pas à "double-sens". Sur la fiche de la donnée associée, il n'y aura pas de **Voir aussi**.

## Résultat dans le front office {#result}

!["Exemple de Voir aussi Dawizz"](/assets/front_metadata_isogeo_saw_dawizz.png)