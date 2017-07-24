---
validated: true
level: 2
---

## Le nombre de requêtes ne doit pas dépasser le nombre moyen des sites du panel WEA (environ 50)

Chaque fichier qui compose une page du site nécessite une requête HTTP.
Cette requête, quelle que soit la taille du fichier va consommer de la bande pasante et du temps.

En dehors des images (qui sont chacune dans un fichier différent), une page HTML pourrait, dans l’idéal, se contenter d’un très petit nombre de fichiers :

* un de contenu (HTML ou XML) ;
* un fichier de mise en forme (CSS ou XSL) ;
* et éventuellement un fichier de traitement (JavaScript) et de police de caractères (WOFF).

L’objectif du développeur sera de minimiser le nombre de ces fichiers (par exemple en concaténant les fichiers de même type) tout en n’augmentant pas le poids de la page.

L'optimisation doit être pensée dès la conception du site.

Les fichiers CSS pour une page pourront être concaténés en un seul (sans pour autant embarquer trop de règles non applicables à la page).
Les fonctions JavaScript utilisées doivent être rassemblées en quelques fichiers.

Tout fichier contenant des données, scripts, polices, etc non utiles à la page doit être supprimé (par exemple, supprimer le chargement d'un script "calendart.js" si la page n'affiche aucun calendrier).

Ne pas oublier, pour aller plus loin, la mise en cache des fichiers utilisés.
