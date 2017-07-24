---
validated: false
level: 2
---

## Mettre en cache les données calculées souvent utilisées

La génération de page à partir de données dynamiques consomme plus de ressources qu'un simple affichage sans recherche ou calcul de données.

Si une recherche de données ou un calcul est fréquement demandé - et surtout si cette recherche (ou calcul) est complexe - il est recommandé de mettre en cache le résultat du coté serveur afin qu'il soit disponible immédiatement.

Il est possible d'utiliser un cache en RAM (key-value store) ou sur un fichier.

Les paramètres conditionnant l'accès aux données mises en cache doivent être soigneusement choisis (les données doivent toujours être à jour et en adéquation avec les restrictions d'accès de l'utilisateur).
