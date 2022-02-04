# Une introduction à PHP

Dans cette section, nous voulons illustrer les principes de base de PHP dans une courte introduction. Ce chapitre traite uniquement de création de pages web dynamiques avec PHP. 

Les pages web qui exploitent PHP sont traitées comme des pages HTML standards, et vous pouvez les créer, éditer et effacer tout comme vous le faites normalement avec des pages HTML classiques.

# Votre première page PHP

Si votre serveur web supporte PHP, vous n'avez rien à faire. Simplement, créez un dossier, puis créez un fichier texte, avec l'extension .php : le serveur va automatiquement l'exécuter avec PHP. Il n'y a pas de compilation.



## Exemple 1 :  Notre premier script PHP : bonjour.php

Créez un fichier appelé *bonjour.php* dans votre dossier web racine (DOCUMENT_ROOT) avec le contenu suivant :

```php
<html>
 <head>
  <title>Test PHP</title>
 </head>
 <body>
 <?php echo '<p>Bonjour le monde</p>'; ?>
 </body>
</html>
```

Utilisez votre navigateur pour accéder au fichier via votre serveur web, en ajoutant le nom de fichier /bonjour.php. Le fichier sera analysé par PHP et le résultat suivant sera envoyé à votre navigateur :

```html
<html>
 <head>
  <title>Test PHP</title>
 </head>
 <body>
 <p>Bonjour le monde</p>
 </body>
</html>
```

Ce programme est extrêmement simple et vous n'avez pas besoin de PHP pour créer une page web comme ceci. Elle ne fait qu'afficher Bonjour le monde, grâce à la fonction *echo* de PHP. Notez que ce fichier n'a pas besoin d'être exécutable ou autre, dans aucun cas. Le serveur sait que ce fichier a besoin d'être interprété par PHP car vous utilisez l'extension ".php", et le serveur est configuré pour les passer à PHP. Voyez cela comme une page HTML normale qui contient une série de balises spéciales qui vont vous permettre de réaliser beaucoup de choses intéressantes.

Le point important de cet exemple était de montrer le format des balises spéciales PHP. Nous avons utilisé ici *<?php* pour indiquer le début de la balise PHP. Puis, nous avons introduit *les commandes PHP* et refermé les balises PHP avec *?>*. Vous pouvez passer du mode PHP au mode HTML et vice-versa, de cette manière, et à votre guise.