---
validated: true
level: 2
---

## Supprimer le code JavaScript redondant

Les sites intégrent des codes JavaScript, soit directement dans le code HTML, soit dans des fichiers externes. Il est possible dans certains cas que le code soit dupliqué plusieurs fois dans la page ou qu’un même fichier soit appelé de multiples fois.

Dans ce cas, le code dupliqué consomme des ressources inutiles (fichiers plus lourds, code interprété plusieurs fois…). Ceci apparait généralement dans le cas de CMS qui peuvent intégrer du code externe (code google analytics, code réseaux sociaux…).

La redondance arrive de plus généralement quand le même code est intégré dans chaque page du site (par exemple le code Google Analytics intégré).

Il est nécessaire de supprimer le code JavaScript redondant dans les sites :

* éviter d’intégrer des codes similaires dans une même page, regrouper pour cela le code redondant dans un fonction commune ;
* éviter le code redondant entre les pages, par exemple, il est utile d’externaliser le code JavaScript du code HTML pour rendre le code commun entre les pages (ce fichier sera de plus mieux géré en cache) ;
* vérifier les multiples inclusions de fichiers (par exemple jQuery), en particulier les inclusions via des plugins dans les CMS.

Exemple de code jQuery inclus 2 fois (dont la deuxième fois par un plugin WordPress) :

```html
<head>
  <script type="text/javascript" src="http://www.monsite.com/wp-includes/js/jquery/jquery.js?ver=1.8.3"></script>
</head>
<body>
  <div class="gmw-map"></div><script type="text/javascript" src="http://www.monsite.com/wp-content/plugins/contact-form-7/includes/js/jquery.form.min.js?ver=3.36.0-2013.06.16"></script>
</body>
```

Il faut vérifier (en regardant le code et les ressources chargées lors du chargement de la page) :

- qu'un code n'est pas répété plusieurs fois sur la même page (plus particulièrement l'inclusion de code comme Google Analytics qui peut être intégré de différentes manières dans les CMS) ;
- qu'un code n'est pas répété entre différentes pages (dans ce cas, il convient de l'externaliser dans un fichier) ;
- qu'un fichier n'est pas appelé plusieurs fois sur la même page.
