# Configuration générale

## Paramètres Isogeo

![](/assets/back_config_api.png)

C'est dans cette section que l'administrateur peut entrer la paire de clés d'authentification oAuth2 transmise afin de permettre au portail de se connecter de façon sécurisée à l'API Isogeo \(`Consumer Key` et `Consumer Secret`\).

Il est fortement recommandé de ne pas modifier les deux autres paramètres `URL oAuth`et `Protocole API` sauf à la demande expresse de votre interlocuteur Isogeo.

---

## Paramètres site

!["Paramètres d'authentification à Isogeo"](/assets/back_config_access.png)On retrouve ici les paramètres généraux d'accès au portail.

### Mail bienvenue

Si l'option est activée, un mail est envoyé à chaque internaute ayant finalisé la procédure de création de compte.

L'objet et le corps du mail sont modifiables dans [le menu`Emails`](/settings/emails.md) du back-office.

### Authentification obligatoire

Quand cette option est activée, le portail n'est accessible qu'aux utilisateurs authentifiés. Le formulaire de connexion s'affiche alors systématiquement à toute personne n'étant pas authentifiée :

!["Configuration de l'accès au portail"](/assets/front_authentification_form.png)

### Google Analytics {#ganalytics}

Si votre portail est accessible sur une URL publique, il est possible d'insérer le code de suivi de fréquentation de l'outil de Google dans ce formulaire.
