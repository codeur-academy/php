# Utiliser un formulaire

L'un des points forts de PHP est sa capacité à gérer les formulaires. Le concept de base qui est important à comprendre est que tous les champs d'un formulaire seront automatiquement disponibles dans le script PHP d'action.

## Exemple - Un simple formulaire HTML

```html
<form action="action.php" method="post">
 <p>Votre nom : <input type="text" name="nom" /></p>
 <p>Votre âge : <input type="text" name="age" /></p>
 <p><input type="submit" value="OK"></p>
</form>
```

Il n'y rien de particulier dans ce formulaire. Il est en HTML pur, sans aucune configuration particulière. Lorsque le visiteur remplit le formulaire, et clique sur le bouton OK, le fichier action.php est appelé. Dans ce fichier, vous pouvez écrire le script suivant :

## Exemple - Afficher des données issues d'un formulaire

```php
Bonjour, <?php echo htmlspecialchars($_POST['nom']); ?>.

Tu as <?php echo (int)$_POST['age']; ?> ans.
```

Voici le résultat que vous pourriez obtenir, selon les valeurs que vous avez saisies :

```html
Bonjour Jean.
Tu as 29 ans.
```

Mis à part les parties *htmlspecialchars()* et *(int)*, ce script ne fait que des choses évidentes.

- htmlspecialchars() s'assure que tous les caractères spéciaux HTML sont proprement encodés afin d'éviter des injections de balises HTML et de Javascript dans vos pages. Pour l'âge, vu que nous savons que c'est un entier, vous pouvez le convertir en un entier. Vous pouvez également demander à PHP de le faire automatiquement à votre place en utilisant l'extension filter. 
- Les variables $_POST['nom'] et $_POST['age'] sont automatiquement créées par PHP. Un peu plus tôt dans ce tutoriel, nous avons utilisé la variable $_SERVER, une superglobale. Maintenant, nous avons introduit une autre superglobale $_POST qui contient toutes les données envoyées par la méthode POST. Notez que dans notre formulaire, nous avons choisi la méthode POST.
  
Si vous aviez utilisé la méthode GET alors notre formulaire aurait placé ces informations dans la variable $_GET, une autre superglobale. Vous pouvez aussi utiliser la variable $_REQUEST, si vous ne souhaitez pas vous embarrasser de la méthode utilisée. Elle contient un mélange des données de GET, POST, COOKIE et FILE.