# Opérations de maintenance

Ce menu, anciennement nommé "Optimisation", permet à l'administrateur.rice du portail de déclencher manuellement les t&#226;ches de maintenance.

## Déverrouiller les objets modifiés {#cleanup_unlock}

Lors de l'édition des différents contenus du portail, un verrou se met automatiquement en place pour protéger ces éléments d'une édition concurrente. Cette section permet à un administrateur de déverrouiller toutes les ressources.

![&quot;Boutons pour déverrouiller les différentes ressources côté back&quot;](/assets/back_unlock.png)

----

## Mots-clés {#cleanup_keywords}

_Fonctionnalité ajoutée avec la _[_version 2.3 du portail_](/versions.html#version23).

Boutons pour forcer le rafraîchissement des mots-clés et de leurs occurrences, utilisés pour le nuage de tags en page d'accueil.

![Mettre &agrave; jour les mots-cl	&eacute;s](/assets/back_keywords_cloud_refresh.png)

----

## Mettre à jour le cache des partages {#cleanup_shares_refresh}

_Fonctionnalité ajoutée avec la _[_version 2.6 du portail_](/versions.html#version26).

Lors d'une modification des partages sur l'interface d'administration Isogeo (<https://app.isogeo.com>), le portail est rafraîchi 1h après.

Ce bouton permet de déclencher manuellement la mise à jour.

![Mettre &agrave; jour les partages](/assets/back_unlock_shares_refresh.png)

> Voir [Paramètres/Affichage](/settings/display.html#display_shares)

----

## Synchronisation avec Isogeo {#cleanup_isogeo_application_sync}

Il peut arriver que les métadonnées présentes dans les catalogues partagés au portail ne soient plus accessibles. Soit parce qu'un adminstrateur Isogeo a modifié les partages, la visibilité de la métadonnée ou la tout simplement supprimée.

La connexion du portail à l'API Isogeo est dynamique et en temps réel, mais si l'administrateur du portail avait utilisé la métadonnée dans des éléments propres au portail \([Sélection de données](/homepage/featured-data.md), [Thématiques](/homepage/thematics.md), [Voir aussi](/settings/voir-aussi.md)...\), cela peut créer un effet "sans issue".

Le bouton `Synchroniser avec Isogeo` permet justement de vérifier que les différentes métadonnées associées aux contenus du portail soient toujours présentes dans le partage. Le cas échéant, elles sont indiquées comme inaccessibles dans les différents menus.

A noter que :

* cette vérification est effectuée quotidiennement de façon automatique côté serveur. Le bouton sert juste à déclencher manuellement le processus.
* le processus peut durer assez longtemps selon le nombre de données concernées.

![Synchroniser avec Isogeo](/assets/back_unlock_share_refresh.png)

----

## Réglages par défaut {#cleanup_factory}

Afin de pouvoir restaurer le portail à état de livraison, le bouton de cette section permettre de remettre à zéro tous les réglagles du back-office.

> ATTENTION : le portail ne dispose d'aucune sauvegarde des paramètres. Il ne sera donc pas possible de revenir à votre configuration une fois ce bouton pressé !

![R&eacute;initialiser les r&eacute;glages d&apos;usine du portail](/assets/back_reset_default.png)

----

## Import les services {#cleanup_geoservices_process}

Afin que l'expérience de consultation du portail soit la plus fluide possible pour l'utilisateur final, le portail génére les URLs de visualisation des services géographiques associés aux métadonnées Isogeo.

Cette routine tourne 3 fois par jour :

* 6h
* 13h
* 20h

Ce menu permet de déclencher manuellement la routine.
