---
validated: true
level: 2
---

## Minimiser le nombre d’iframes

Réduire le nombre d’iframes dans le code source, voire s’en passer si possible.

Une iframe qui ne répond pas peut bloquer le site.
On ne peut contrôler le contenu de l’iframe, il n’y a donc aucune action d’optimisation sur les images ou les scripts possibles : une iframe peut donc allonger les temps de chargement.

Les bonnes pratiques à appliquer sont :

- supprimer les iframes inutiles ;
- préférer l'utilisation de webservices en remplacement des iframes si le service cible le propose ;
- charger l'iframe de manière asychrone, sur requête de l'utilisateur de préférence.

Notation :
- 2 points si aucune iframe n'est présente sur le site ;
- 1 point s'il y a une iframe ;
- 0 point s'il y a strictement plus d'une iframe.
