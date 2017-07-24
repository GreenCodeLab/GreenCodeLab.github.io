---
validated: true
level: 1
---

## Mettre en cache le favicon.ico

Éviter une demande de téléchargement du favicon.ico systématique à chaque page et qui, de plus, peut générer une erreur.

Le favicon.ico est recherché par les navigateurs ; il change peu, il doit donc être présent, et être l’objet de règles de cache pour ne pas être redemandé trop souvent.

Il est recommandé que le fichier favicon.ico :

- soit le même fichier pour toutes les pages du site ;
- soit bien défini dans les entètes de chaque page du site ;
- soit mis en cache par le navigateur client.

De plus, il est possible d'optimiser le fichier et ne pas y cumuler plusieurs tailles différentes superflues.
