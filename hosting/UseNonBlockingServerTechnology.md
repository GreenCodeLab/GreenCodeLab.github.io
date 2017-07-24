---
validated: true
level: 2
---

## Utiliser un serveur avec une technologie non bloquante

Les serveurs web classiques sont généralement basés sur des technologies « thread » (par exemple Apache). Avec ces technologies, lorsqu’il y a des visiteurs concurrents, les ressources matérielles sont allouées pour chaque utilisateur tant que les données ne sont pas transmises. Énormement de mémoire est par exemple utilisée.

Les serveurs de type non bloquant permettent un usage plus efficient des ressources matérielles.

Il est nécessaire d’utiliser des technologies non bloquantes et basées sur des événements pour les serveurs web.

Exemple de solutions non bloquantes : Nginx, Jetty.
