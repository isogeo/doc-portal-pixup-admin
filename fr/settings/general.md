---
description: Gérer les paramètres généraux du portail Isogeo
---
# Paramètres généraux

Cette section comporte les paramètres généraux du site. Tous les paramètres avec une * sont obligatoires.

## Accès au site {#site_access}

### Accès réseau {#network}

Ce paramètre permet de désactiver les captcha lorsque portail est installé sur une machine déconnectée d'internet.

### Accès certificat {#certificat}

Ce paramètre permet d'indiquer le chemin vers le certificat lorsque le portail utilise l'API Isogeo en mode On-premises.

![Renseigner le chemin vers le certificat](/assets/back_distant_certificate.png)

> NB : Laissez l'option `Certificat distant` dans le cas de l'utilisation de l'API Isogeo en mode SaaS.

### Maintenance {#maintenance}

Valeurs possibles :

* Le géoportail est accessible
* Le géoportail est en maintenance

Il est donc possible de prévenir l'utilisateur d'une maintenance du portail. Dans ce cas, le portail affiche l'image ci-dessous.

![Message  de maintenance aux utilisateurs](/assets/front_maintenance.png)

### Extracteur {#extractor}

Ce paramètre permet d'activer le panier et l'extracteur de données du Portail. Il faut au préalable partager les mêmes données aux deux applications dans l'interface d'administration (cf. [Partages](https://app.isogeo.com/groups/admin/shares/)).

Si activé, il faut indiquer l'url de l'extracteur soit par défaut : https://extractor.isogeo.com/portal/cart

### Authentification {#authentication}

Valeurs possibles :

* La consultation du géoportail est libre
* L'authentification est requise pour consulter le géoportail

Il est donc possible de forcer les utilisateurs à s'authentifier au portail pour accéder à son contenu. Il s'agit d'une sécurité pour les portails qui ne souhaitent pas être ouverts au public par exemple.

![Authentification obligatoire](/assets/front_authentication.png)

### Type d'authentification {#authentification_type}

Ce paramètre permet de déléguer la création et l'authentification des utilisateurs à un gestionnaire d'identité SaaS comme AzureAD (cf. [Paramétrage de l'application AzureAD](/appendices/azuread.md)) ou Okta en indiquant les paramètres fournis par l'outil correspondant.

![Paramétrage de l'authentification AzureAD](/assets/back_authentication.png)

NB > Vous pouvez conserver la possibilité de s'authentifier avec le gestionnaire d'utilisateur natif du portail en selectionnant `Oui` pour le paramètre `Avec login Isogeo`.

### Création de compte

Ce paramètre permet de choisir si les utilisateurs peuvent demander la création d'un compte ou si elle est réservée aux administrateurs.

### Nom du site {#site-name}

Le nom du site choisi s'affiche dans le titre de l'onglet de votre navigateur. 

### Debug {#debug}

Cette option est réservée à l'équipe Isogeo et permet d'afficher des messages de debug sur le portail.

### Envoi de mail {#send_email}

Cette option permet de désactiver l'envoi de mail et masque les menus de configuration [des mails d'envoi/reception](#reception_emails) et du [serveur de courriel utilisé](#mail_server).

### Restriction IP

Ce menu de configuration permet d'autoriser l'accès au portail à une liste d'IP sélectionnées. Il suffit d'indiquer les adresses IP les unes en dessous des autres avec un retour à la ligne. 

NB > Cette restriction ne s'applique qu'au front. L'interface d'admin est toujours accessible avec authentification à l'adresse https://nomportail.domain.ext/admin. Ce qui peut être bien utile en cas d'erreur de saisie d'IP...

----

## API {#api}

> **Attention, ces paramètres sont réservés à l'équipe Isogeo.**

Il s'agit de tous les paramètres concernant les API Isogeo et Dawizz.

* API utilisée : cocher la case `Dawizz` pour activer l'API Dawizz. Sinon, seule l'API Isogeo est utilisée par défaut.
* Isogeo Consumer Key : Identifiant d'authentification à l'API Isogeo
* Isogeo Consumer Secret : Clé d'authentification à l'API Isogeo
* Dawizz API Key : Clé de l'API Dawizz. Ce champ est obligatoire si vous utilisez l'API Dawizz pour accéder à votre catalogue de données.
* Isogeo URL oAuth : URL de l'API Isogeo (par défaut: https://id.api.isogeo.com/oauth/token)
* Isogeo URL APP : URL de l'application Isogeo (par défaut: http://app.isogeo.com)
* Isogeo Protocole API * : URL du protocole de l'API Isogeo (par défaut: https://v1.api.isogeo.com)
* Isogeo Url GeoDataProcess : URL de l'API Geodataprocess Isogeo utilisée pour l'exploitation des services géographiques

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

Il est possible d'utiliser son propre serveur de mails pour l'envoi des notifications ci-dessus.
Ceci est très pratique pour passer les multiples sécurités informatiques mises en place au sein de votre organisme.

Il faut donc renseigner les champs suivants :

* Hôte
* Port
* Identifiant
* Mot de passe : le mot de passe ne s'affichera plus une fois enregistré. Le laisser donc vide si inchangé.
* SMTP Secure

> N'hésitez pas à contacter le support Isogeo (support@isogeo.fr) en cas de problème de configuration du serveur de mail.

## Javascript et CSS {#ganalytics}

Si votre portail est accessible sur une URL publique, il est possible d'insérer le code de suivi de fréquentation de l'outil de Google, de Matomo ou autre dans ce formulaire.

Vous pouvez également insérer des balises CSS ou de code javascript (réservé aux utilisateurs avancés).
