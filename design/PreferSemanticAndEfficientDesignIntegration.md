---
validated: true
level: 1
---

## Favoriser une intégration du design sémantique et efficace

Une architecture de code complexe ou une mise en page brouillonne augmentera la quantité de données transférées ainsi que la consommation électrique du site via son usage.

En effet, soit à cause du temps de calcul du navigateur, soit à cause du temps de lecture par un utilisateur qui trouve difficilement ses informations, le poste client restera plus longtemps en activité et, forcément, consommera davantage.

La notion de design couvre aussi à la fois celui du code HTML vu par le navigateur et la mise en page vue par l’utilisateur du site.

Le design du code, quant à lui, doit utiliser au mieux les recommandations des normes W3C.
Les balises HTML doivent être utilisées au minimum, dans un but de séparation sémantique des données et pas dans un but de mise en page.
La mise en page se fait uniquement dans les fichiers CSS, de manière indépendante.

En ce qui concerne le design de la mise en page, celle-ci doit être cohérente sur tout le site afin que l’utilisateur trouve aisément les informations mises à sa disposition.

Les techniques utilisées peuvent être les suivantes :

- utiliser des balises sémantiques HTML5 (_nav_, _header_, _footer_, _article_, etc) et éviter les balises _div_ ;
- ne pas placer de règles de style à l'intérieur des balises (utiliser un fichier CSS ou placer les règles de styles en entête HTML) ;
- séparer distinctement les zones de la page selon leurs fonctions (menu principal, ancres, articles, infos complémentaires, etc) ;
- ne pas afficher plus de contenu sur la page que ce que voulait lire l'utilisateur (par exemple, éviter de cumuler une liste d'articles sur 4 hauteurs d'écran) ;
- proposer un plan de site simple permettant à l'utilisateur d'accéder rapidement à toutes les informations du site.

Pour la vérification de cette règle, il est possible de chiffrer :

- le code HTML et la proportion de balise par rapport au texte ;
- la profondeur maximum du DOM (par la vue 3D des outils de développement de Firefox par exemple) ;
- le nombre de styles de pages différentes pour un contenu de même type sémantique ;
- le nombre d'informations de natures différentes sur une même page (un texte, un portfolio, une liste, un tableau comparatif et une liste de liens sur une même page seront à recharger à chaque fois que l'on veut consulter les liens).
