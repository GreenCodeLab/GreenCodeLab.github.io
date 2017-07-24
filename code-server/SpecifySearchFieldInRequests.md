---
validated: true
level: 1
---

## Préciser la colonne de recherche lors des requêtes

Minimiser la quantité de données lors de la réponse à une requête et minimiser le travail du serveur de base.

Le serveur de base de données consommera plus de CPU et de mémoire pour chercher lui-même la liste des champs d’un objets et tous les renseigner que de traiter une liste de champs spécifiée.

Éviter d'écrire :

```sql
SELECT * FROM objet ..
```

Préférer :

```sql
SELECT nom, description, dimension FROM objet WHERE ...
```

Si le site web audité utilise un CMS, la règle s'applique uniquement au code éventuellement développé en plus du CMS.
