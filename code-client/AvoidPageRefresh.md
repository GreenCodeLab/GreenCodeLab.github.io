---
validated: true
level: 1
---

## Ne pas rafraîchir les pages

Il est possible de demander le rafraîchissement d’une page internet régulièrement via la balise metadata avec l’attribut Refresh : &lt;meta http-equiv="name" content="bar"&gt;.
Cela permet de mettre à jour la page (par exemple pour recharger des publicités).

Cependant cela est coûteux car toute la page est rechargée. Même si le cache est utilisé, il y aura des requêtes et des traitements.

L’utilisation de &lt;meta http-equiv="name" content="bar"&gt; devrait être interdite. Si un rafraîchissement est nécessaire, il est préférable d’utiliser des technologies comme AJAX.

De la même manière, l’utilisation de JavaScript doit être évitée afin de recharger la page.
