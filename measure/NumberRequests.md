---
validated: true
level: 2
---

## Le nombre de requêtes ne doit pas dépasser le nombre moyen des sites du panel WEA (50)

Chaque fichier qui compose une page du site nécessite une requête HTTP.
Cette requête, quelle que soit la taille du fichier va consommer de la bande pasante et du temps.

En dehors des images (qui sont chacune dans un fichier différent), une page HTML pourrait, dans l’idéal, se contenter d’un très petit nombre de fichiers :

* un de contenu (HTML ou XML) ;
* un fichier de mise en forme (CSS ou XSL) ;
* et éventuellement un fichier de traitement (JavaScript) et de police de caractères (WOFF).

L’objectif du développeur sera de minimiser le nombre de ces fichiers (par exemple en concaténant les fichiers de même type) tout en n’augmentant pas le poids de la page.
