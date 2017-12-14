# Utilisateurs

Isogeo distingue plusieurs profils utilisateurs :

* Super Admin

Le super Admin peut administrer et configurer tout le portail Isogeo via l'[interface d'administration](http://demo.isogeo.net/admin/menu.php?menu_item=dashboard). Il a également tous les droits de consultation de façon à pouvoir vérifier toutes ses modifications. 

* Admin rédacteur

L' admin rédacteur a lui aussi accès à l'[interface d'administration](http://demo.isogeo.net/admin/menu.php?menu_item=dashboard). Cependant il ne peut modifier que le contenu du portail \(actualités, menus...\). 

* Utilisateur privilégié

L'utilisateur privilégié est un utilisateur particulier qui peut jongler entre le portail Isogeo et l'[application Isogeo](https://app.isogeo.com/). En effet, sur une fiche de métadonnée, il dispose du lien vers la fiche de métadonnées "mère" dans l'application Isogeo. S'il possède les droits de modification, il peut donc éditer directement la fiche de métadonnées puis consulter ses modifications dans le portail. En revanche cet utilisateur n'a pas accès à l'interface d'administration. 

* Utilisateur authentifié 

L' utilisateur authentifié peut utiliser la plupart des fonctionnalités du portail. Il peut consulter les  fiches de métadonnées, la carte, les actualités etc... 

## Matrice du type d'utilisateur

Voici ci-dessous les fonctionnalités ouverte en fonction du type d'utilisateur. 

ATTENTION : Il s'agit des fonctionnalités par défaut. L'affichage de certaines informations et certaines fonctionnalités sont modifiables par le super administrateur dans les [paramètres de gestion de l'affichage selon les profils](https://isogeo.gitbooks.io/app-portal-pixup-admin/content/settings/display.html). 

| Fonctionnalités | Super Admin | Admin rédacteur | Utilisateur privilégié | Utilisateur authentifié |
| :--- | :---: | :---: | :---: | :---: |
| Effectuer une recherche | X | X | X | X |
| Afficher une métadonnées | X | X | X | X |
| Accéder à la carte | X | X | X | X |
| Télécharger une ressource | X | X | X | X |
| Créer une liste | X | X | X | X |
| Sauvegarde une fiche dans une liste | X | X | X | X |
| Envoyer des commentaires | X | X | X | X |
| Lire les actualités | X | X | X | X |
| Contacter les administrateurs | X | X | X | X |
| Gérer son compte \(Listes, paramètres, licences, mot de passe\) | X | X | X | X |
| Accéder au lien vers la fiche dans app.isogeo de façon à l'éditer si autorisation | X | X | X |  |
| Partager une fiche en iframe | X | X | X |  |
| Accéder à l'interface d'administration | X | X |  |  |
| Visualiser les statistiques du portail \(dashboard\) | X | X |  |  |
| Configurer les actualités \(ajout, édition, suppression\) | X | X |  |  |
| Configurer les médias \(images, fichiers\) | X | X |  |  |
| Gérer les pages \(pied de page\) | X | X |  |  |
| Configurer la page d'accueil | X |  |  |  |
| Gérer les messages et les commentaires | X |  |  |  |
| Configurer les menus | X |  |  |  |
| Gérer les paramètres \(généraux, affichage, emails, recherche...\) | X |  |  |  |
| Consulter les statistiques dans le détails | X |  |  |  |
| Gérer les utilisateurs \(Ajout, droits\) | X |  |  |  |

## Créer un nouvel utilisateur

Pour créer un nouvel utilisateur, il faut donc se connecter à l'interface d'administration en mode "Super Admin".

Etapes :

1. Cliquer sur l'onglet Utilisateurs, puis [Nouvel Utilisateur](http://demo.isogeo.net/admin/users/edit_user.php?IDItem=-1&menu_item=edit_user).
2. Remplir la fiche descriptive de l'utilisateur \(Attention à bien choisir les droits en fonction de la matrice ci-dessus\).
3. Cliquer sur Enregistrer.

L'utilisateur peut ensuite se connecter immédiatement avec l'adresse mail et le mot de passe que vous avez enregistré dans le descriptif. Il convient à l'utilisateur de modifier son mot de passe à sa première connexion.

Pour cela :

1. Connectez-vous avec vos identifiants au portail.
2. Cliquez sur votre nom d'utilisateur à coté de la barre de recherche.
3. Dans **PARAMETRES** cliquez sur "Cliquez ici pour modifier votre mot de passe".
4. Ecrivez votre mail, vous devriez recevoir le message automatique ci-dessous.
5. Cliquez sur le lien "Cliquer ici'.
6. Puis changez votre mot de passe.
7. Validez.

![](/assets/Capture_chgt_mdp_potail_mail.PNG)

![](/assets/Capture_chgt_mdp_portail.PNG)

