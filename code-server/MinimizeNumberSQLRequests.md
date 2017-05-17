---
validated: true
level: 1
---

## Minimiser le nombre de requêtes SQL

Une connexion à une base de données, quel que soit son type (SGBD, système de fichier, …) est coûteux en ressources processeur, mémoire et réseau pour l’architecture du serveur.
Cette règle évite de trop nombreuses connexions à une base.

Si une boucle effectue une requête à chaque itération, ceci dégradera la performance et l’empreinte globale du site.

Il est donc nécessaire d’exclure toute requête de toute boucle itérative.

On pourra aussi par exemple utiliser des transactions.
