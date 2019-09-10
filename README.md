# Isogeo - Portal documentation

[![Build Status](https://dev.azure.com/isogeo/Documentations/_apis/build/status/isogeo.doc-portal-pixup-admin?branchName=master)](https://dev.azure.com/isogeo/Documentations/_build/latest?definitionId=31&branchName=master)

Content, structure and media of the website documentation. It's part of the Isogeo online documentations ([see Github repositories](https://github.com/search?q=topic%3Adocumentation+org%3Aisogeo&type=Repositories)).

## Edit this documentation

It's based on Gitbook v3.2.* which is:

* [a book format](https://github.com/GitbookIO/gitbook)
* [a toolchain](https://toolchain.gitbook.com/)

## Deployment

It's deployed on Isogeo Azure (Storage v2 Static website) using Azure DevOps ([see config](https://github.com/isogeo/doc-portal-pixup-admin/blob/master/azure-pipelines.yml)):

* QA:
  * <https://qaisogeohelp.z28.web.core.windows.net/pixup-portal/>
  * <http://help.qa.isogeo.com/pixup-portal/>
* PROD:
  * <https://prodisogeohelp.z28.web.core.windows.net/pixup-portal/>
  * <http://help.isogeo.com/pixup-portal/>

Deployment rules:

* each commit triggers a deployment on QA
* each tagged commit triggers a deployment on PROD - [see tags](https://github.com/isogeo/doc-portal-pixup-admin/tags)

See: <https://github.com/isogeo/doc-homepage/wiki>
