# Voir aussi

Pour faciliter la découverte et la navigation dans les catalogues partagés, le portail intègre un système de suggestions des métadonnées potentiellement similaires à celle que l'utilisateur est en train de consulter.

Exemple de résultat :

![](/assets/front_similarity_result_manual_3items.PNG)

## Fonctionnement

Une fois le chargement de la métadonnée en mode détaillé terminé, le système tire au sort l'un des mots-clés et effectue une recherche filtrée dessus. Une fois la métadonnée actuelle exclue du résultat de recherche, plusieurs cas de figure se présentent alors :

* s'il y a plus d'un résultat, jusqu'aux 3 premières métadonnées similaires sont affichés en bas de la métadonnée ;
* s'il n'y a aucun résultat, rien n'est affiché.

C'es notamment pour pouvoir gérer ce dernier cas \(mais aussi pour "forcer" la similarité\), l'administrateur du portail peut configurer des "Voir aussi" manuellement.

## Créer un "Voir aussi" manuel

Voici la procédure à suivre :

1. Se rendre dans le menu `Voir aussi` ;
2. Cliquer sur `Créer un nouveau voir aussi` ;
3. Dans le premier champ, coller l'URL complète de la fiche : les 3 champs suivants se mettent alors à jour pour permettre de vérifier qu'il s'agit de la bonne fiche ;
4. Dans les 3 derniers champs, ajouter les identifiants uniques des métadonnées à lier.
5. Cliquer sur `Enregistrer`.

![](/assets/back_similarity_manual_add.png)



