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

De nombreux CMS n'obligeant pas l'utilisation d'une base de données pour accéder aux pages et à leur contenu existent (PluXml, CMSimple, Zwii...).

Dans le cas de recherche de données dans une page, le rythme des connexions à la base de données doit être en phase avec le rythme d'actualisation souhaité des données sources plutôt qu'avec le rythme d'accès.
C'est à dire qu'il est recommandé de mettre en cache les résultat d'une requête pour les restituer aux postes clients sans faire de nouvelles connexions.

Dans le cas de connexions servant à contruire l'URL d'une page ou l'accès à un fichier, il est recommandé d'en exclure toute utilisation ne servant qu'à trouver des fichiers "statiques" tels que les images (\*.jpg, \*.png) et les fichiers de codes (\*.js, \*.css, etc).

Cette règle ne permet un calcul strict, mais permet de noter l'engagement de l'audité à faire baisser l'empreinte de sa page.
L'audité doit être en mesure de justifier sa politique d'utilisation de base données.
Par exemple, le nombre de connexions par accès aux pages doit être estimé, controlé et des moyens d'améliorations doivent avoir été évalués.
