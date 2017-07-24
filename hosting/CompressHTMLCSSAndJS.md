---
validated: true
level: 1
---

## Compresser la sortie HTML, CSS et JS

Diminuer la taille des pages générées en utilisant la compression fournie par les serveur web.

L’activation de moteurs de compression (deflate/gzip pour Apache, gzip pour Ngnix…) permet de réduire le poids de la page en compression les données envoyées au navigateur.

Exemple sous Apache : activer et paramétrer les modules "a2enmod headers" et "a2enmod deflate".

Il faut vérifier la présence de l'entête "Content-Encoding: gzip" dans la réponse HTTP.
