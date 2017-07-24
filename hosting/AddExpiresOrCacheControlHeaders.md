---
validated: true
level: 1
---

## Ajouter des entêtes Expires ou Cache-Control

Il est possible de diminuer la quantité de fichier transmise sur le réseau en forçant la mise en mémoire cache par le navigateur des fichiers du site.

Lors de sa première visite d’un site, le navigateur reçoit tous les fichiers nécessaires à l’affichage de la page.
La plupart de ces fichiers seront utilisés à nouveau, non seulement lors d’une consultation de cette même page mais aussi lors de la consultation d’autres pages du site.

Il est donc très intéressant que le site demande une mise en cache de tous les fichiers qui resteront inchangés entre deux consultations du site.

Les fichiers à mettre en cache sont, a minima, tous les fichiers statiques.
Lors de la configuration du serveur, ils seront identifiables par leurs extensions :

- fichiers correspondants à des images (jpg, png, giff, jpeg, ico) ;
- fichiers contenant du texte ou des données :(html, xml) ;
- fichiers de mise en forme de ces données (css, xsl, xslt) ;
- fichiers de traitements à effectuer par le navigateur (js, swf) ;
- fichiers des polices de caractères (eot, woff, svg).

La configuration de la gestion du cache est effectuée dans la configuration du serveur HTTP (directives "Header set Cache-Control") ou dans les entêtes des fichiers HTML (ou PHP) eux-mêmes (balises Expires ou Cache-Control).
