---
description: Hébergement et accès des portails Isogeo
---
# Accès au portail en HTTPS

Afin de garantir la sécurité des informations transmises lors de l'authentification des utillisateurs ou des requêtes à l'API Isogeo ainsi que pour optimiser le [référencement](//appendices/seo.md), le portail de données gère le HTTPS \(depuis la [version 2.4](/versions.md#version24)\).

## Portails hébergés par Isogeo {#hosted}

La procédure se base sur un échange entre Isogeo et l'organisme client, qui est généralement en charge de son nom de domaine :

1. Isogeo envoie un fichier  CSR \(_Certificate Signing Request_ - voir [wikipédia](https://fr.wikipedia.org/wiki/Demande_de_signature_de_certificat)\) lié au nom de \[sous-\]domaine correspondant au portail \(typiquement geocatalogue.organisme.fr\).
2. l'organisme client génére le certificat à partir du CSR et l'envoie au format .zip à Isogeo.
3. Isogeo installe le certificat et indique l'adresse IP vers laquelle doit pointer le nom de domaine.
4. L'organisme client fait pointer la zone DNS de son nom de domaine vers l'adresse IP transmise.

---

## Portails hébergés par les clients {#intranet}

Dans ce cas là, le client est responsable de l'installation des certificats. Le portail détectera automatiquement le HTTPS et se chargera de la redirection.