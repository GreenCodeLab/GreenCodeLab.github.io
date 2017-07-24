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

Si une boucle est nécessaire, il est recommandé :

- d'utiliser la boucle uniquement pour préparer les données nécessaires aux requêtes ;
- d'effectuer la requête après la boucle en accumulant les transactions (insertion ou modifications ou suppressions) dans une même requête.

Par exemple, pour supprimer une liste d'objets, éviter d'écrire :

```php
foreach ($objectIdsList as $objet) {
  $query = "DELETE FOM $objetTable WHERE $id = $objet";
  mysql_query($query);
}
```

Il est préférable d'écrire :

```php
$objectIds = '('. implode (',',$objectIdsList). ')';
query =  "DELETE FOM $objetTable WHERE $id IN $objectIds";
mysql_query($query);
```

Si le site web audité utilise un CMS, la règle s'applique uniquement au code éventuellement développé en plus du CMS.
