---
validated: true
level: 1
---

## Appliquer une alternative textuelle aux images

Les images doivent systématiquement posséder un attribut alt.

L’attribut alt doit être vide si l’image est décorative, porteur de sens si l’image est informative. Un attribut alt absent, ou renseigné alors qu’il devrait être vide posera des problèmes de restitutions par les aides techniques (lecteur vocal, etc).

Chaque image (img, object, area, etc) doit posséder un attribut alt :

```html
<img alt="description_image" />
```
