# Gestion de l'affichage selon les profils {#display_rights}

Le portail permet de gérer une granularité de 5 niveaux sur les différentes parties des métadonnées.

Exemples de cas d'usage :

* selon son niveau d'accès, un utilisateur ne voit pas les même métadonnées.
* définir qu'un utilisateur non authentifié ne verra pas les attributs, alors qu'un utilisateur authentifié (connecté avec son identifiant/mot de passe) pourra les voir.

![Paramètres d&apos;affichage selon le niveau d&apos;accès d&apos; utilisateur](/assets/back_display_advanced_user.png)

---

## Options

### Métadonnées visibles selon les partages {#display_shares}

| Paramètre            | Description |
| :------------------- | :---------- |
| Partages accessibles | Partage affecté au groupe d'utilisateur. Si rien n'est sélectionné, l'utilisateur voit l'ensemble des métadonnées partagées au portail (= tous les partages).  |

Si une modification est faite dans APP (exemple : une fiche est enlevée du catalogue public), il faut [mettre à jour le cache des partages](/settings/unlock.md#cleanup_shares_refresh) pour que la fiche ne soit plus visible dans le portail pour le profil d'utilisateur concerné.

Sinon, la modification sera effective au bout d'une heure (tâche planifiée).

### Informations sur les différentes parties du portail {#display_site_parts}

| Paramètre | Description |
| :-------- | :---------- |
| Afficher propriétaire | Permet d'indiquer où le nom du groupe de travail ayant créé la métadonnée s'affiche dans les différentes interfaces du portail : page d'accueil \(dans [les pavés dynamiques](/homepage/dyn-sections.md)\), résultats de rechecrhe \(menu Catalogue par défaut\) et sur le détail d'une fiche de métadonnées. |
| Afficher échelle | Pareil que le paramètre précédent mais avec la valeur du champ [Echelle](https://help.isogeo.com/fr/features/documentation/md_geography.html#echelle) d'Isogeo. |
| Afficher type | Pareil que le paramètre précédent mais avec la valeur du champ [Type](https://help.isogeo.com/fr/features/documentation/index.html#les-différents-types-de-ressources) d'Isogeo. |
| Intitulé "Propriétaire" | Permet de changer l'intitulé du groupe de travail qui a créé la fiche de métadonnées dans Isogeo, pour éviter les confusions. Correspond au champ [Propriétaire](https://help.isogeo.com/fr/start/group_switch.html#mon-compte-mes-groupes-de-travail) d'Isogeo. Valeur par défaut : _Propriétaire de la métadonnée_. |

---

### Actions disponibles sur une métadonnée {#display_actions}

| Paramètre | Description |
| :-------- | :---------- |
| Boutons fonctionnalités | Permet de définir le style des boutons d'actions présents sur une fiche de métadonnées \(télécharger, visualiser...\). Soit sous forme de texte ![Boutons - textes](/assets/front_md_actions_labels.png) , soit sous forme d'icônes \(avec le texte en infobulles\) ![Boutons - icones](/assets/front_md_actions_buttons.png). |
| Copier le chemin | Donne la possibilité de copier le chemin d'accès à la donnée dans le presse-papiers. |
| Partager avec iFrame | Donne la possibilité d'obtenir le code de partage iFrame pour intégrer la fiche directement dans un autre site web. |
| Noter une fiche | Donne la possibilité de noter la fiche - Indisponible pour les utilisateurs publics |
| Commenter une fiche | Donne la possibilité de commenter la fiche - Indisponible pour les utilisateurs publics |

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
