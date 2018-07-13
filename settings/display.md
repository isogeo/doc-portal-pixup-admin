# Gestion de l'affichage selon les profils {#display_rights}

L'administrateur choisissant les catalogues partagés au portail directement depuis la plateforme Isogeo, on considère alors que toutes les métadonnées ont vocation à être diffusées aux personnes ayant accès au portail. Mais toutes les informations contenues dans les métadonnées ne concernent pas tous les utilisateurs.

Le portail permet de gérer une granularité de 5 niveaux sur les différentes parties des métadonnées. Par exemple, il est posible de définir qu'un utilisateur non authentifié \(internaute ou intranaute donc\) ne verra pas les attributs, alors qu'un utilisateur authentifié \(connecté avec son identifiant/mot de passe\) pourra les voir.

![&quot;Exemple des paramètres d&apos;affichage pour le rôle &apos;Utilisateur authentifié avec privilège&apos;&quot;](/assets/back_display_advanced_user.png)

---

## Options

### Informations sur les différentes parties du portail {#display_site_parts}

| Paramètre | Description |
| :--- | :--- |
| Afficher propriétaire | Permet d'indiquer où le nom du groupe de travail ayant créé la métadonnée s'affiche dans les différentes interfaces du portail : page d'accueil \(dans [les pavés dynamiques](/homepage/dyn-sections.md)\), résultats de rechecrhe \(menu Catalogue par défaut\) et sur le détail d'une fiche de métadonnées. |
| Afficher échelle | Pareil que le paramètre précédent mais avec la valeur du champ [Echelle](http://help.isogeo.com/fr/features/documentation/md_geography.html#echelle) d'Isogeo. |
| Afficher type | Pareil que le paramètre précédent mais avec la valeur du champ [Type](http://help.isogeo.com/fr/features/documentation/index.html#les-différents-types-de-ressources) d'Isogeo. |
| Intitulé "Propriétaire" | Permet de changer l'intitulé du groupe de travail qui a créé la fiche de métadonnées dans Isogeo, pour éviter les confusions. Correspond au champ [Propriétaire](http://help.isogeo.com/fr/start/group_switch.html#mon-compte-mes-groupes-de-travail) d'Isogeo. Valeur par défaut : _Propriétaire de la métadonnée_. |

---

### Actions disponibles sur une métadonnée {#display_actions}

| Paramètre | Description |
| :--- | :--- |
| Boutons fonctionnalités | Permet de définir le style des boutons d'actions présents sur une fiche de métadonnées \(télécharger, visualiser...\). Soit sous forme de texte ![](/assets/front_md_actions_buttons.png) , soit sous forme d'icônes \(avec le texte en infobulles\) ![](/assets/front_md_actions_labels.png). |
| Copier le chemin | Donne la possibilité de copier le chemin d'accès à la donnée dans le presse-papiers. |
| Partager avec iFrame | Donne la possibilité d'obtenir le code de partage iFrame pour intégrer la fiche directement dans un autre site web. |
| Noter une fiche | Donne la possibilité de noter la fiche. |
| Commenter une fiche | Donne la possibilité de commenter la fiche. |

---

### Sections des métadonnées {#display_metadata_sections}

| Paramètre            | Description |
| :------------------- | :---------- |
| Attributs            | Affiche le tableau des attributs des données vectorielles. |
| Conditions           | Affiche les licences. |
| Contacts             | Affiche les contacts. |
| Couches de services  | Affiche le bouton de visualisation des services géographiques liés. |
| Evénements           | Affiche les 5 derniers événements intervenus sur les données. |
| Infos techniques     | Affiche le bloc Informations techniques. |
| Limitations          | Affiche les limitations. |
| Note                 | Affiche la note de la métadonnée. |
| Ressources associées | Affiche les boutons d'actions. |
| Spécifications       | Affiche les spécifications. |
| Voir aussi           | Affiche la section ["Voir Aussi"](/settings/voir-aussi.md). |
