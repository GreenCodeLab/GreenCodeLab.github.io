---
validated: true
level: 1
---

## Préférer le texte brut au HTML lors de l’envoi des mails

Si le site prévoit des envois d’e-mails, et d’autant plus s’il s’agit d’envois fréquents ou nombreux, il est recommandé de ne transmettre que le minimum d’information nécessaire.
Ceci peut diviser en moyenne par 4 le poids des messages envoyés.

Les mails envoyés par le serveur doivent se contenter de données sous forme texte seul, respectant les règles suivantes :

- ne pas ajouter de mise en forme (titres, polices, tableaux, listes, etc) ;
- ne pas systématiquement ajouter d'images (logo, signatures, photos, etc) ;
- utiliser "Content-Type : text/plain".

Il est possible de laisser le choix (texte ou HTML) à l'utilisateur.
