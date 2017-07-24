---
validated: true
level: 2
---

## Ne pas charger de données lourdes si elles ne sont pas visibles

Le but est de diminuer le poids total des éléments téléchargés en se limitant aux données visibles.
Ceci n’a de sens que si le volume de données non visibles (images, graphiques) est important.

Dans les cas où la longeur de la page est bien supérieure à la hauteur de la fenêtre du navigateur et que la quantité de données à afficher est importante, il est possible de ne pas afficher les données (images) non visibles.

Cette fonctionnalité est permise par la technique du *lazy loading*, qui n'est cependant pas native dans les navigateurs.
Il faudra donc soit utiliser du code JavaScript, soit utiliser une bibliothèque.

Cette technique se base sur l'utilisation de la fonction "getBoundingClientRect" d'un élément en la comparant avec la propriété "innerHeight" de la fenêtre du navigateur.

Ce fonctionnement peut aussi s'appliquer si la fenêtre n'est pas visible (chargement dans un onglet).

Attention à ne pas charger un fichier JavaScript contenant toute une librairie de fonctions si seule la fonction de *lazy loading* est utile.
