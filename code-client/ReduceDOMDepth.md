---
validated: true
level: 2
---

## Réduire la profondeur du DOM

Simplifier le DOM (Document Object Model) économisera du traitement (affichage, mise en forme, traitement JavaScript) par le navigateur client.

Le DOM doit être le plus simple possible.
Son arborescence doit être limité et ne pas développer de profondeurs inutiles.
Les éléments disponibles en HTML5 rendent possible un code HTML lisible et facile à mettre en forme en CSS sans créer des « boîtes » inutiles.

Les mauvaises pratiques suivantes doivent être évitées :

- présence d'éléments HTML sans sémantique particulière (par exemple "div") ne contenant qu'un seul objet ;
- présence déélements de type "div" s'empilant les uns dans les autres sans ajout de texte ou de données.

Notation : 2 points pour une profondeur maximale du DOM <=10, 1 point pour une profondeur maximale du DOM <=15.
