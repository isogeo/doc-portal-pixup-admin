---
description: Gérer les paramètres généraux du portail Isogeo
---
# Paramètres généraux

Cette section comporte les paramètres généraux du site. Tous les paramètres avec une * sont obligatoires.

## Accès au site {#site_access}

### Maintenance {#maintenance}

Valeurs possibles :

* Le géoportail est accessible
* Le géoportail est en maintenance

Il est donc possible de prévenir l'utilisateur d'une maintenance du portail. Dans ce cas, le portail affiche l'image ci-dessous.

![Message  de maintenance aux utilisateurs](/assets/front_maintenance.png)

### Authentification {#authentication}

Valeurs possibles :

* La consultation du géoportail est libre
* L'authentification est requise pour consulter le géoportail

Il est donc possible de forcer les utilisateurs à s'authentifier au portail pour accéder à son contenu. Il s'agit d'une sécurité pour les portails qui ne souhaitent pas être ouverts au public par exemple.

![Authentification obligatoire](/assets/front_authentication.png)

### Nature du géoportail {#nature}

Valeurs possibles :

* Portail géomatique
* Portail marketing

Selon le choix, la page d'accueil du site sera respectivement la [page d'accueil métier](/homepage-jobs/titles.md) ou la [page d'accueil marketing](/homepage-marketing/widget-marketing/titles.md).

### Nom du site {#site-name}

Le nom du site choisi s'affiche dans le titre de l'onglet de votre navigateur. 

----

## API {#api}

> **Attention, ces paramètres sont réservés à l'équipe Isogeo.**

Il s'agit de tous les paramètres concernant les API Isogeo et Dawizz.

* API utilisée : cocher la case `Dawizz` pour activer l'API Dawizz. Sinon, seule l'API Isogeo est utilisée par défault.
* Isogeo Consumer Key : Identifiant d'authentification à l'API Isogeo
* Isogeo Consumer Secret : Clé d'authentificaiton à l'API Isogeo
* Dawizz API Key : Clé de l'API Dawizz. Ce champ est obligatoire si vous utilisez l'API Dawizz pour accéder à votre catalogue de données.
* Isogeo URL oAuth : URL de l'API Isogeo (par défault : https://id.api.isogeo.com/oauth/token)
* Isogeo URL APP : URL de l'application Isogeo (par défault : http://app.isogeo.com)
* Isogeo Protocole API * : URL du protocole de l'API Isogeo (par défault : https://v1.api.isogeo.com)

----

## Ressources externes {#extern_ressources}

> **Attention, ces paramètres sont réservés à l'équipe Isogeo.**

Il s'agit des clés client et serveur qui permettent d'utiliser le Captcha Google (cf. capture ci-dessous) dans tous les formulaires du site soit :

* Formulaire de création de compte
* Formulaire de contact
* Formulaire de l'onglet discussion d'une fiche de métadonnée pour les utilisateurs non identifiés

![Captcha Google](/assets/front_captcha.png)

> Pour information, obtenir ces clés auprès de Google est gratuit et se fait [à cette adresse](https://www.google.com/recaptcha/admin/).

----

## Réseaux sociaux {#social_network}

Il est possible de renseigner les liens vers les réseaux sociaux de votre organisme. On retrouve ensuite ces liens dans le pied de page du site. 

!["Retrouvez-nous sur..."](/assets/front_social_network.png)

----

## Comptes mails utilisés pour l'envoi et la réception {#reception_emails}

Ce menu concerne les messages envoyés par les utilisateurs via le formulaire de contact dans le menu du site `Contact`(cf. capture ci-dessous).

!["Formulaire de contact](/assets/front_contact.png)

Les administrateurs reçoivent une notification par mail selon la configuration de ces paramètres.

* Courriel réception : adresse mail de réception des notifications (obligatoire)
* Courriel réception 2 : adresse mail de réception des notifications (facultative)
* Courriel réception 3 : adresse mail de réception des notifications (facultative)
* Courriel expéditeur : `ne-pas-repondre@isogeo.com` (par défaut)
* Nom expéditeur * :  `Geoportail Isogeo` (par défaut)

Voici le résultat de la notification par mail avec les paramètres par défaut.

![Notification par mail](/assets/notif_mail_contact.png)

----

## Serveur de courriels {#mail_server}

Il est possible d'utiliser son propre serveur de mail pour l'envoi des notifications ci-dessus.
Ceci est très pratique pour passer les multiples sécurités informatiques mises en place au sein de votre organisme.

Il faut donc renseigner les champs suivants :

* Hôte
* Port
* Identifiant
* Mot de passe : le mot de passe ne s'affichera plus une fois enregistré. Le laisser donc vide si inchangé.
* SMTP Secure

## Google Analytics {#ganalytics}

Si votre portail est accessible sur une URL publique, il est possible d'insérer le code de suivi de fréquentation de l'outil de Google dans ce formulaire.
