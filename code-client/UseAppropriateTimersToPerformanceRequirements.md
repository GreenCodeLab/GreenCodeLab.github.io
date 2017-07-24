---
validated: true
level: 1
---

## Utiliser des timers les plus adéquats aux exigences de performance

Les systèmes d’exploitation possèdent des timers périodiques qui séquencent les traitements. Par exemple, Microsoft Windows séquence ses tâches avec un timer de 15,6 ms. Si aucun traitement n’est nécessaire, le processeur se réveille puis entre dans un mode de veille. Certaines applications (comme les applications multimédias) diminuent ce timer pour avoir une performance plus importante.

Cela a un impact sur la consommation du processeur car il entre moins souvent en veille.

Il faut limiter l’usage de fonctions qui augmente le timer des systèmes. Par exemple on évitera l’usage de setTimeout() ou setInterval() avec des variables inférieures à 10 ms.

Exemple d'usage à éviter, affichant l'heure toutes les 5 ms :

```js
var myVar = setInterval(function(){myTimer()},5);

function myTimer() {
    var d = new Date();
    document.getElementById("demo").innerHTML = d.toLocaleTimeString();
}
```

Dans le cas d'un timer inférieur à 10 ms, l'usage doit être justifié (fonction graphique par exemple).
