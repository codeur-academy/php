# Une introduction à PHP

- PHP est un langage de programmation pour la création de la programmation back-end des pages web.
  - Son interfaçage avec la base de données MySQL permet d'élaborer des applications rapides, avec une actualisation en temps réel des données. 
  - Installer PHP est la solution pour stoker et afficher des milliers d'informations sur vos sites web.

- Les principaux avantages à installer un script PHP
  - Exécution record des scripts coté serveur.
  - Protections des scripts.
  - Langage gratuit en Open Source.
  - Simplicité d'interfaçage avec des systèmes de bases de données comme MySQL.

- Architecture CLIENT- SERVEUR
  - Votre navigateur est le CLIENT. 
    - C'est lui qui demande la page web au serveur... et le client se fournit dans la base de donnée de fonctions et de contenus du serveur. 

- Description d'une requête HTTP basique :
  - Le navigateur envoi au serveur, qui héberge le site, l'adresse que vous avez tapé dans la barre d'adresses de votre navigateur.
  - Le serveur retourne après traitement le contenu de la page à votre navigateur
  - Observation :
    - Avec ou sans PHP, le serveur traite la demande et retourne la page. 
    - Additionner du PHP au traitement n'a aucune incidence sur le parcours basique de la requête http. 
    - Le serveur va se charger de traiter vos scripts PHP et se chargera aussi du traitement des données de vos tables SQL, avant de renvoyer la page terminée à votre navigateur.
  - Coté SERVEUR
    - Le PHP est interprété directement et uniquement par le serveur. 
    - Les aspirateurs ne peuvent pas aspirer des pages PHP. 
    - Celle-ci sont protégées contre le téléchargement par le serveur. 
    - La seule manière d'accéder à vos pages PHP est par un client FTP / SSH comme Filezilla ou Putty .
  - Le serveur ne renvoi que des données (le résultat des traitements de requêtes ou de fonctions..) ce qui constitue le source de la page (HTML, JavaScript, CSS, etc. + des informations sur les headers...) à la machine du client.

- Les différents langages comme le HTML, JavaScript ou CSS sont des langages CLIENTS.
  - Les scripts de ces différents langages sont téléchargés sur votre ordinateur et ensuite interprétés par votre navigateur.

- Base de données
  - MySQL analyse et exécute le code SQL. 
  - PHP sert de support pour envoyer des requêtes au serveur MySQL.
  - phpMyAdmin est une administration en Open Source pour administrer votre base de données MySQL.














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