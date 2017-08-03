# Présentation générale

Le portail de données est une application tierce de la plateforme Isogeo, dédiée à la valorisation de l'information géographique. 



L’OpenCatalog est l’un des modules historiques de la plateforme Isogeo. En permettant à ses administrateurs de partager rapidement et facilement leur catalogue de ressources SIG sur le web, il offre la possibilité à des utilisateurs de plus en plus nombreux de découvrir un patrimoine de données à leur disposition. Cependant OpenCatalog a peu évolué depuis 3 ans. Que ce soit sur le plan de son ergonomie comme de ses fonctionnalités, aucune évolution notable a été mise en ligne. En ne permettant pas de choisir entre une diffusion maîtrisée ou public de ses catalogues, OpenCatalog ne remplit pas complètement sa mission. Enfin, dans certains cas, il est difficile d’accéder aux ressources cataloguées.

Dans ce contexte, il a été décidé de lui “refaire une jeunesse” et d’en faire un véritable média d'accès aux données en interne comme en externe. Ce travail se fera en deux versions. La version 2.3 est spécifiée dans ce document. Elle s’attachera surtout à revoir la recherche, la navigation dans le catalogue et à permettre l’extraction de données servies en WFS. La version 3.0 s'attellera au niveau de diffusion et à l'accès aux données en interne. Elle sera décrite dans une autre série de spécifications et ne sortira pas en 2017.

Ce chantier est l'occasion pour l’équipe Isogeo de spécifier le produit en mode “atelier” ou tout le monde est consulté et peut apporter sa “pierre à l’édifice”. C’est aussi une occasion pour le futur développeur frontend de “se faire la main” sur la plateforme Isogeo.

# Vision

La vision d’OpenCatalog est légèrement modifiée afin d’intégrer la diffusion de données non géographiques :

Pourles clients Isogeo

Quiveulent diffuser leurs métadonnées géographiques et non géographiques à un public divers et maîtrisé,OpenCatalog

Estun site web en accès libre

Quipermet aux administrateurs d'ouvrir un ou plusieurs de leurs catalogues à un public choisi de spécialistes et de non spécialistes des SIG qui veulent découvrir et accéder à des données géographiques pour les consommer ou les visualiser.Catalogue par catalogue, les administrateurs peuvent choisir une diffusion maîtrisée à des utilisateurs qui disposent d'un lien spécifique ou une diffusion publique qui permet de rassembler toutes les fiches de métadonnées, par catalogue et par organisme, de manière ouverte et indexable par les moteurs de recherche courants \(Google, Bing...\).Tout ou partie d'OpenCatalog est intégrable tel quel dans un portail via la technologie IFRAME. Dans OpenCatalog une fiche de métadonnées recense tous les services d'accès publics à la donnée sous-jacente. OpenCatalog n'est pas un outil de création de services \(cartographie, extraction...\).

# Objectifs

* Revoir la recherche \(filtre, tri, auto-complétion, etc.\)

* Revoir la présentation des fiches de métadonnées \(ajout d’une vignette, modification de la mise en page, possibilité de déplier/replier la liste des attributs, etc.\)

* Permettre la navigation entre les fiches de données et de services

* Permettre l’extraction de données servies en WFS \(choix du format, du système de coordonnées et de l’emprise selon les capacités du service\)

* Permettre la visualisation de couches WFS “pur” et de couches WMTS



