---
validated: true
level: 2
---

## Mettre en cache le bytecode

Optimiser le traitement par le serveur des scripts et programmes en langages interprétés.

Sur le serveur, les programmes en langages interprétés (PHP, Perl, Python, …) sont stockés sous leur forme originale (texte).
Le serveur doit, à chaque exécution, interpréter le langage avant son exécution.
Ceci donne du travail supplémentaire au serveur et ajoute du temps d’attente au poste client.

Pour chaque langage, des solutions différentes peuvent exister.
Le premier type de solution consiste à obtenir un fichier exécutable pré-compilé (par exemple, "HipHop for PHP" pour le langage PHP).)
Le deuxième type de solution est que le serveur mette en cache le bytecode (exécutable) obtenu à la première exécution du script pour s'en servir lors des exécutions suivantes (par exemple, "Alternative PHP Cache" pour PHP).

L'audité doit décrire la solution mise en place et son champ d'action pour les scripts du site (systématique, pour quelques script ou répertoires, etc).
