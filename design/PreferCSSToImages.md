---
validated: true
level: 1
---

## Préférer les CSS aux images

Minimiser la quantité d’octets utilisés en utilisant les capacités graphiques du navigateur plutot que de transférer des images.

Les images les plus simples, compressées et utilisant une palette de couleur minimum auront une taille de fichier dépassant largement le kilo-octets. Cette taille peut aller facilement à 10 voir plusieurs centaines de kilo-octets. Cette charge sera à transférer lors de la lecture de la page sur le poste client.

Les navigateurs possèdent des capacités de création d’objets graphiques en interprétant des codes texte de mise en page (le CSS).
Ces objets graphiques vont des simples rectangles colorés et augmentés de bordure pour le CSS2 jusqu’à des objets arrondis, en 3D et avec des dégradés de couleurs pour le CSS3 désormais courramment interprété.

Utiliser des objets définis par CSS remplace plusieurs fichiers de plusieurs milliers d’octets par quelques lignes de codes de plusieurs dizaines (au plus centaines d’octets). Ce code étant rassemblé dans un seul fichier, l’économis s’étend aussi au coût du transfert HTTP pour chaque image.
