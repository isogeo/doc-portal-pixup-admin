# Optimisation \(anciennement Déverrouillage\)

## Déverrouiller les objets modifiés

Lors de l'édition des différents contenus du portail, un verrou se met automatiquement en place pour protéger ces éléments d'une édition concurrente. Cette setion permet à un administrateur de déverrouiller toutes les ressources.

![&quot;Boutons pour déverrouiller les différentes ressources côté back&quot;](/assets/back_unlock.png)

## Mots-clés

Boutons pour forcer le rafraîchissement des mots-clés et de leurs occurences, utilisés pour le nuage en page d'accueil.

## Mise à jour du partage Isogeo

Il peut arriver que les métadonnées présentes dans les catalogues partagés au portail ne soient plus accessibles. Soit parce qu'un adminstrateur Isogeo a modifié les partages, la visibilité de la métadonnée ou la tout simplement supprimée.

La connexion du portail à l'API Isogeo est dynamique et en temps réel, mais si l'administrateur du portail avait utilisé la métadonnée dans des éléments propres au portail \([Sélection de données](/homepage/featured-data.md), [Thématiques](/homepage/thematics.md), [Voir aussi](/settings/voir-aussi.md)...\), cela peut poser des problèmes.

Le bouton `Vérifier les données du partage Isogeo` permet justement de vérifier que les différentes métadonnées associées aux contenus du portail soient toujours présentes dans le partage. Le cas échéant, elles sont indiquées comme inaccessibles dans les différents menus.

A noter que :

* cette vérification est effectuée quotidiennement de façon automatique côté serveur. Le bouton sert juste à déclencher manuellement le processus.
* le processus peut durer assez longtemps selon le nombre de données concernées.



