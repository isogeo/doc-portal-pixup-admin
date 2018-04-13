# Accès au portail en HTTPS

Afin de garantir la sécurité des informations transmises lors de l'authentification des utillisateurs ou des requêtes à l'API Isogeo ainsi que pour optimiser le [référencement](//appendices/seo.md), le portail de données gère le HTTPS \(depuis la [version 2.4](/versions.md#version24)\).

## Portails hébergés par Isogeo {#hosted}

Voici la procédure :

1. Isogeo envoie un fichier  CSR \(_Certificate Signing Request_ - voir wikipédia\) et le transmettre au client

---

## Portails hébergés par les clients {#intranet}

Dans ce cas là, le client est responsable de l'installation des certificats. Le portail détectera automatiquement le HTTPS et se chargera de la redirection.

