# Paramètres d'affichage selon le type d'utilisateur

Pour chaque niveau de droit, *Super Admin*, *Admin Rédacteur*, *Utilisateur avec privilèges*, *Utilisateur authentifié* et *Utilisateur public* il est possible de paramétrer toutes les paramètres ci-dessous.

## Nombre de résultats par page {#nb-result-page}

Le nombre doit être compris entre 10 et 100 par pas de 10.

## Partages accessibles {#shares}

Il est possible de créer plusieurs partages dans l'[interface d'administration d'Isogeo](https://app.isogeo.com/admin/shares) puis de choisir le ou les partages accessibles par niveau de droit.

Si aucun partage n'est sélectionné, toutes les données partagée à l'application *Portail* sont accessibles.

### Exemple d'utilisation de la fonctionnalité {#shares-example}

1. Partager le *catalogue de données interne* dans un partage à destination du portail et le rendre accessible aux utilisateurs suivants :
  * Super Admin
  * Admin Rédacteur
  * Utilisateur avec privilèges
  * Utilisateur authentifié

2. Créer un autre partage vers le même portail contenant le *catalogue de données public* et le rendre accessible à l'utilisateur public.

## Copier le chemin {#copy-path}

Cette fonctionnalité permet d'autoriser la copie de l'emplacement de la ressource de la fiche de métadonnées si celui-ci est un chemin (exemple : `D:\SIG\DATA\REFERENCE\IGN\BDTOPO\`).

Cette fonctionnalité peut être utile dans le cadre d'un portail interne dans lequel les utilisateurs ont accès aux données SIG via des répertoires partagés.

Lorsque l'emplacement est accessible, le bouton ci-après s'affiche à coté de la croix sur une fiche de métadonnées. ![](/assets/front_button_copy_path.png)

## Partager avec iFrame {#share-iframe}

Cette fonctionnalité active la possibilité de copier un iFrame intégrant la métadonnée concernée.

Lorsque le partage avec iFrame est activé, le bouton ci-après s'affiche à coté de la croix sur une fiche de métadonnées. ![](/assets/front_button_copy_iframe_1.png)

En cliquant, un code intégrable en iFrame dans un site web est automatiquement généré (cf. Capture ci-dessous).

!["Code iFrame à intégré dans une page web"](/assets/front_button_copy_iframe.png)

## Noter une fiche {#note}

L'utilisateur peut noter une fiche de métadonnée en cliquant sur le nombre d'étoiles qu'il souhaite affecter (cf. capture ci-dessous).

!["Noter une fiche dans le front office"](/assets/front_note.png)

## Consulter les notes {#note-consulting}

Si oui, l'utilisateur peut visualiser les notes sur les fiches de métadonnée.

## Masquer les données de type "Services" (API Isogeo) {#services}

Cette fonctionnalité permet de masquer les fiches de services dans le catalogue et le filtre correspondant. En revanche, elles sont toujours comptabilisées dans le nombre de résultat de la recherche.

!["Résultats dans le front office lorsque les fiches de services sont masquées"](/assets/front_without_services.png)

> Cette fonctionnalité ne concerne que les portails dont la recherche utilise l'API Isogeo.

## N'afficher que les données publiées (API Dawizz) {#dawizz-published-datas}

Cette fonctionnalité permet d'afficher uniquement les données ayant le statut "*Publiée*" dans le catalogue Dawizz partagé au portail. Pour afficher toutes les données, sélectionner *Afficher les fiches pour lesquelles ce paramètre n'est pas renseigné*.

!["Données publiées dans l'interface Dawizz"](/assets/dawizz_data_published.png)

> Cette fonctionnalité ne concerne que les portails dont la recherche utilise l'API Dawizz.

## Affichage personnalisé des métadonnées

### Champs visibles à plusieurs endroits {#multiple-fields}

Cette section permet de gérer l'affichage de certains champs sur :

* la page d'accueil
* les résultats de la recherche (= vignette d'aperçu de la métadonnée)
* le détail d'une fiche.

On peut donc choisir d'afficher ou non l'interprétation du markdown et les champs suivants :

* Markdown
* Propriétaire
* Echelle
* Type

!["Back office - Affichage des champs"](/assets/back_markdown.png)

#### Résultats sur le front office {#mutiple-fields-result}

Sont représentés ci-dessous les résultats sur le front office lorsque tout est activé ou désactivé.

* Sur la page d'accueil

!["Sur la page d'accueil lorsque tout est activé"](/assets/front_markdown_homepage_active.png)

!["Sur la page d'accueil lorsque tout est désactivé"](/assets/front_markdown_homepage_desactive.png)

* Sur les résultats de recherche

!["Sur les résultats de recherche lorsque tout est activé"](/assets/front_markdown_research_active.png)

!["Sur les résultats de recherche lorsque tout est désactivé"](/assets/front_markdown_research_desactive.png)

* Sur le détail d'une fiche

!["Sur le détail d'une fiche lorsque tout est désactivé"](/assets/front_markdown_metadata_active.png)

!["Sur le détail d'une fiche lorsque tout est désactivé"](/assets/front_markdown_metadata_desactive.png)

### Onglets des fiches de métadonnées {#tabs}

Vous pouvez choisir ici d'afficher ou non les onglets ci-dessous selon le profil d'utilisateur.

#### Description

##### Fiches Isogeo {#isogeo-description}

Pour les fiches Isogeo, l'onglet description présente la plupart des champs de métadonnées

* Résumé
* Information techniques
  * Propriétaire
  * Nom de la couche
  * Nombre d'entités
  * Type de géométrie
  * Résolution
  * Échelle
  * Format de référence
  * Système de coordonnées
  * Encodage des caractères
  * Contexte de collecte
  * Méthode de collecte
* Qualité (conformité aux spécifications)
* Règle de topologie
* Conditions d'accès et d'utilisation
  * Licence
  * Description de la licence
* Limitations
  * Directive
  * Contenu
  * Restriction
  * Description
* Contacts
  * Point de contact
  * Autres rôles de contact

!["Onglet Description d'une fiche Isogeo"](/assets/front_isogeo_description.png)

##### Fiches Dawizz {#dawizz-description}

Pour les fiches Dawizz, on retrouve les champs suivants

* Description
* Mots-clés et thématiques
* Référent(s)
* Concepts de thesauri
* Application
* Descriptif de l'application
* Type de donnée
* Domaine de l'application
* Nombre d'attributs
* Nombre d'enregistrements
* Date de création de la fiche de métadonnée
* Date de dernière mise à jour
* Langue

!["Onglet Description d'une fiche Dawizz"](/assets/front_dawizz_description.png)

#### Événements {#events}

On retrouve dans cet onglet les champs concernant l'historique de la donnée et la timeline des derniers évènements sur la donnée.

* Historique de la donnée
  * Date de création
  * Date de dernière modification
  * Début de validité
  * Fin de validité
  * Fréquence de mise à jour
* Derniers événements sur la donnée
  * Date de publication
  * Date de mise à jour
  * Date de création

!["Onglet Evénements d'une fiche Isogeo"](/assets/front_isogeo_events.png)

#### Visualisation {#visualization}

Cet onglet permet de visualiser les données lorsque qu'un ou plusieurs service(s) est(sont) associé(s) à la fiche de métadonnée dans Isogeo.

!["Onglet Visualisation d'une fiche Isogeo"](/assets/front_metadata_visualisation.png)

> NB : Le pré-chargement des couches est géré dans un cache ([voir ici comment gérer ce cache](/fr/services/import.md)).

#### Téléchargement {#download}

Cet onglet permet de télécharger la métadonnée ou la donnée elle-même lorsqu'un lien de téléchargement est renseigné dans la fiche de métadonnée.

* Fiche au format XML
* Fiche au format PDF

!["Onglet Téléchargement d'une fiche Isogeo"](/assets/front_metadata_download.png)

#### Attributs {#attributes}

##### Fiche Isogeo {#isogeo-attributes}

Présentation des attributs sous forme de tableau avec les colonnes suivantes :

* Nom
* Alias
* Type
* Description
* Langue

!["Onglet Attributs d'une fiche Isogeo"](/assets/front_metadata_isogeo_attributes.png)

##### Fiche Dawizz {#dawizz-attributes}

Présentation des attributs des fiches Dawizz sous forme de tableau avec les colonnes suivantes :

* Index
* Identifiant
* Type
* Analyse des titres
* Analyse des concepts

!["Onglet Attributs d'une fiche Dawizz"](/assets/front_metadata_dawizz_attributes.png)

#### Discussion {#tchat}

Cet onglet permet de visualiser les fils de discussion existants ou d'en créer un.

!["Onglet Discussion d'une fiche Isogeo"](/assets/front_metadata_isogeo_tchat.png)

#### Voir aussi {#see-as-well}

Cet onglet permet de visualiser les données ajoutées au "Voir-aussi" par l'administrateur. (cf. [Voir Aussi Isogeo](/see-as-well/s_a_w_isogeo.md)).

!["Onglet Voir aussi d'une fiche Isogeo"](/assets/front_metadata_isogeo_saw.png)

### Détails des fiches de métadonnées {#metadata-details}

* Événements : afficher/masquer la timeline des derniers évènements (cf. [Onglet Evénements](#events))
* Spécifications : afficher/masquer les spécifications (cf. [Onglet Description - Qualité](#isogeo-description))
* Conditions : afficher/masquer les conditions (cf. [Onglet Description - Conditions d'accès et d'utilisation](#isogeo-description))
* Limitations :  afficher/masquer les limitations (cf. [Onglet Description - Limitations](#isogeo-description))
* Contact :  afficher/masquer les contacts (cf. [Onglet Description - Contacts](#isogeo-description))
* Chat actif : active/désactive l'accès au tchat. Si le tchat est désactivé, l'utilisateur peut quand même envoyer un message à l'administrateur (cf. Capture ci-dessous).

!["Formulaire de contact de l'onglet Discussion lorsque le tchat est désactivé"](/assets/front_metadata_tchat_desactive.png)

> Le *Tchat* ne peut être activé qu'aux utilisateurs authentifiés sur la plateforme. Il n'est donc pas accessible aux utilisateurs publics.

### Pavés des fiches de métadonnées {#cobblestones}

#### Pavé "Mots-clés" {#keywords}

Lorsque le pavé des mots-clés est affiché, l'utilisateur accède aux mots-clés et peut naviguer automatiquement vers la recherche filtrée sur le mot-clé en cliquant dessus.

!["Pavé des mots-clés activé"](/assets/front_metadata_keywords.png)

> NB : Le lien vers la recherche filtrée correspondante n'est pas disponible sur les portails utilisant l'API Dawizz.

#### Pavé "Thèmes Inspire" {#inspire}

Lorsque le pavé des thèmes Inspire est affiché, l'utilisateur accède aux thèmes Inspire et peut naviguer automatiquement vers la recherche filtrée sur le thème Inspire en cliquant dessus.

!["Pavé des thèmes Inspire activé"](/assets/front_metadata_inspire.png)

> NB : Le lien vers la recherche filtrée correspondante n'est pas disponible sur les portails utilisant l'API Dawizz.

#### Pavé "Listes" {#list}

Le pavé *Listes* permet à l'utilisateur de créer des listes ou d'ajouter la donnée consultée à une liste existante. 

!["Pavé des listes activé"](/assets/front_metadata_list.png)

> Le pavé "Liste" ne peut être activé qu'aux utilisateurs authentifiés sur la plateforme. Il n'est donc pas accessible aux utilisateurs publics.

### Filtre de recherche {research-filters}

#### Filtres Isogeo {#isogeo-filters}

Il est possible de sélectionner les filtres affichés selon l'utilisateur et de choisir leur ordre d'affichage.

* Filtre "Types de données"
* Filtre "Mots-clés"
* Filtre "Thèmes Inspire"
* Filtre "Actions"
* Filtre "Contacts"
* Filtre "Formats"
* Filtre "Licenses"
* Filtre "Thématiques"
* Filtre "Systèmes de coordonnées"

!["Choisir l'ordre des filtres Isogeo"](/assets/back_order_research_filters.png)

#### Filtres Dawizz {#dawizz-filters}

Il en est de même pour les filtres Dawizz lorsque l'API Dawizz est utilisée bien entendu.

* Filtre "Thesaurus"
* Filtre "Applications"
* Filtre "Formats"
* Filtre "Mots-clés"
* Filtre "Réseau"
* Filtre "Serveurs"
* Filtre "Statuts"
* Filtre "Thématiques"
* Filtre "Types"