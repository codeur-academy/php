# Qu'est ce que PHP?

PHP (Hypertext Preprocessor) est un langage de scripts généraliste et Open Source, spécialement conçu pour le développement d'applications web. Il peut être intégré facilement au HTML.

Bien... mais qu'est ce que cela veut dire ? Un exemple :

Exemple 1 : Exemple d'introduction

```php
<!DOCTYPE html>
<html>
<head>
<title>Exemple</title>
</head>
<body>

<?php
echo "Bonjour, je suis un script PHP !";
?>

</body>
</html>
```

Ce code affiche "Bonjour, je suis un script PHP !"). 

Le code PHP est inclus entre une balise de début <?php et une balise de fin ?> qui permettent au serveur web de passer en mode PHP.

Ce qui distingue PHP des langages de script comme le Javascript, est que le code est exécuté sur le serveur, générant ainsi le HTML, qui sera ensuite envoyé au client. Le client ne reçoit que le résultat du script, sans aucun moyen d'avoir accès au code qui a produit ce résultat. 

Le grand avantage de PHP est qu'il est extrêmement simple pour les néophytes, mais offre des fonctionnalités avancées pour les experts. 