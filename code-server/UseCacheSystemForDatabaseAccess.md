---
validated: true
level: 2
---

## Utiliser un système de cache pour l’accès à la base de données

Une connexion à une base de données, quel que soit son type (SGBD, système de fichier, …) est couteux en ressources processeur, mémoire et réseau pour l’architecture du serveur.
Il est donc important de pouvoir éviter les connexions dès que cela est possible.

Plusieurs cas d’utilisation de données sont possibles : la recherche de données dans une page ou la recherche d’adresse de page ou de fichier (pour certains CMS).

Dans un premier temps, le choix du type de base doit s’adapter au besoin. Une base de données relationnelle ne sera efficace qu’au delà d’un millier de données. D’autre part il n’est pas avantageux d’utiliser un CMS incluant un SGBD pour, par exemple, simplement une dizaine de pages de présentation.

Ensuite, si une base est nécessaire, son utilisation doit se faire sous un controle maitrisé et justifié.
