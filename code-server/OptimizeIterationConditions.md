---
validated: true
level: 1
---

## Optimiser les conditions d’itération

Diminuer le nombre de traitements par le serveur lors d’une itération à l’intérieur d’un script.

Lors d’une itération, il est recommandé de calculer à l’avance toutes les variables utilisées dans la boucle et qui resteront stables.
Ceci évite de refaire, lors des conditions de sortie (ou même à l’intérieur de l’itération), des calculs inutiles car déjà connus.

Par exemple, remplacer :

```php
for ($i=0 ; $i < count($liste) ; $i++) {
  echo $liste[$i];
}
```

par :

```php
$count = count($liste);
for ($i=0 ; $i < $count ; $i++) {
  echo $liste[$i];
}
```
