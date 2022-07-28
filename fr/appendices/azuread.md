# Paramétrage de l'application AzureAD

Il est possible de gérer l'authentification des utilisateurs du Portail directement depuis votre Active Directory AzureAD.

1. Depuis la page d’accueil du [Portail Azure](https://portal.azure.com/#home), aller dans "Autres Services" puis choisir "Inscriptions d’applications" :

![Services Azure](/assets/AzureAD/services.png)

2. Inscrire une nouvelle application selon la configuration ci-dessous

![Inscrire une application](/assets/AzureAD/register_application.png)

3. Récupérer les informations suivantes :
  
ID d’application (parfois appelé « client ID »)
ID de l’annuaire (parfois appelé « tenant »)

![Détail de l'application](/assets/AzureAD/application_detail.png)

4. Créer un nouveau secret client dans le menu Certificats & secrets :

ATTENTION : cet élément n’est lisible et copiable/collable qu'immédiatement après avoir été créé. On ne peut plus ensuite le récupérer, la seule solution étant alors de créer un nouveau secret client.

![Créer un nouveau secret](/assets/AzureAD/new_client_secret.png)

5. Ouvrir le menu Authentification
6. Ajouter une plateforme de type Web
7. Indiquer les url(s) de connexion et de deconnexion et cocher la case "Jetons d’accès (utilisés pour les flux implicites)"

![Configuration des urls](/assets/AzureAD/configure_url.png)

8. Renseigner les informations récupérées (Annuaire ID, Application ID et Secret Client) dans les paramètres généraux du Portail en choisissant le type d'authentification Azure AD

![Configuration des paramètres Azure AD dans le back-office](/assets/AzureAD/back_office_azuread_configuration.png)

Vous pouvez choisir de conserver également le système d'authentification natif du Portail. Les deux solutions seront ansi proposées côté front.

![Se connecter avec Azure AD sur le front](/assets/AzureAD/front_azuread_authentication.png)
