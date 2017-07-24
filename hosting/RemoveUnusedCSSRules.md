---
validated: true
level: 1
---

## Supprimer les règles CSS inutilisées

Minimiser le poids des fichiers CSS en supprimant les règles ou les fichiers CSS qui ne correspondent pas aux objets du site consulté.

Les fichiers CSS tranférés avec la page ne doivent pas contenir de règles inutilisés dans le site (ou au mieux dans la page).
Il est important que les fichiers CSS, venant par exemple de démos ou importés d’autres sites, ne soient pas utilisés sans y supprimer toutes les règles non utilisés.

Les règles non utilisés sont, par exemple, des règles sur des objets du DOM inexisants dans le site.
Ces règles peuvent correspondent à des identifiants, tags ou classes non utilisés ou à des hierarchies d'objets non existantes.
Elles peuvent aussi correspondre à des états d'objets jamais vérifiés ou encore à des objets dont la règle "display:none" s'applique.

Il peut être utile de vérifier aussi la pertinence de la factorisation des fichiers CSS.
Trop de fichiers va impacter le nompbre de requêtes HTTP tandis qu'un seul fichier ne peut voir qu'un faible pourcentage de règles concernées pour la page active.
