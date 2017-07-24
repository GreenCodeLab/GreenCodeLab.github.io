---
validated: true
level: 2
---

## Désactiver les modules qui ne sont pas utilisés

Charger des modules (JavaScript, CSS, ou autres librairies) augmente le poids total de la page. Or, ce poids joue sur la consommation du poste client et des équipements du réseau entre le serveur et chaque poste client.

En plus de diminuer le poids des images, des requêtes HTTP inutiles et du JavaScript redondant, le code peut être optimisé pour ne pas charger de librairies ou de codes CSS inutiles.

Tout en faisant attention de ne pas multiplier le nombre de pages, il est possible de ne charger que ce qui est nécessaire à la page.
Le principe à appliquer est équivalent pour les fichiers CSS ou les fichiers JS : il s'agit d'organiser une conception modulaire du site.

Les fonctions et règles CSS devront être découpées en modules.
Ces modules concerneront les fonctions utiles à plusieurs pages en excluant celles qui ne sont pas utilisées.

Le développeur doit prouver son approche modulaire.
Il est possible de vérifier un corollaire de cette règle : ne pas intégrer de code JS ou CSS dans une page HTML alors que les fonctions ou règles peuvent être utilisées par d'autres pages.
