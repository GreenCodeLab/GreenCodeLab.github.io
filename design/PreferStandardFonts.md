---
validated: true
level: 1
---

## Favoriser les polices standards

Éviter de surcharger les téléchargements avec des fichiers de polices de caractères.

Le besoin d’un site d’une lecture fluide et d’une identité visuelle étant prise en compte, des chargements inutiles et répétés de polices de caractères à chaque page du site est une erreur à éviter.

La première solution pour optimiser le téléchargement des polices d'un site est de n'utiliser que des polices standards, pré-installées dans les navigateurs.
Cette solution a ses limites car chaque système d'exploitation a des polices standards différentes, dont le rendu pourra être différent.

S'il est choisi d'utiliser des polices spécifiques, il est alors nécessaire de :

- minimiser le nombre total de polices utilisées sur le site ;
- s'assurer que les polices chargées seront mises en cache par le navigateur ;
- s'assurer de ne charger qu'un seul fichier par police utilisée (eot, woff, etc selon le navigateur) ;
- choisir les fichiers de police les moins lourds à télécharger (comparer les tailles des fichiers woff et svg par exemple) ;
- utiliser si possible les capacités du navigateur pour "grasser" les polices plutôt que de charger des fichiers différents pour chaque épaisseur ;
- ne télécharger que les polices réellement utilisées sur la page du site.

Il est possible d'attribuer tous les points pour cette règle même s'il existe des polices spécifiques (dans ce cas, tous les points listés ci-dessus doivent être vérifiés).
