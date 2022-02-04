#  unité pourcentage

Dans ce travail pratique nous allons découvrir l’unité relative pourcentages.

Nous allons comprendre aussi, la notion de l’héritage des valeurs de l’élément père vers ces éléments fils. 

Comme d'habitude nous avons besoin d'un fichier HTML avec le code de l'article d’exemple. 

Maintenant la taille de police de notre paragraphe est 32 pixels.
 Si nous lui attribuons la valeur 100%, il va prendre la valeur 100 % de la taille de police de l'élément père body.

Mais, puisque l’élément body ne possède pas une règle pour font-size, il va hérité cette valeur de son père, car la valeur de la propriété font-size peut être hérité.

Aussi, l'élément HTML ne possède pas une règle pour la propriété font-size, dans ce cas il prend la valeur par défaut qu’est égale 16px. 

Donc, la taille de police du paragraphe va prendre 16px, 

Pour la clarté de notre exemple, nous allons fixer la taille de police de notre élément racine HTML. On peut lui attribuer la valeur 32px.

Dans ce cas, cette valeur va être héritée par l’élément body, et notre paragraphe va prendre 100 % de cette valeur, c’est à dire 32px.

Maintenant, si nous changeons la valeur de font-size de l’élément body à 16px

Notre paragraphe va prendre 16px et non 32px.

Si, nous attribuons la valeur 16px à l’élément HTML et la valeur 20px à l’élément body, 
notre paragraphe prend la valeur 20px qu’est égale à la valeur de son père.


Les valeurs pourcentage ne sont pas appliquées seulement à la propriété font-sizee, il peuvent-être appliquer aussi à d'autres propriétés comme par exemple l’hauteur et la largeur.

Puisque nous allons travailler sur les dimensions de notre paragraphe, je vous propose de changer sans arrière-plan pour plus de clarté et de visibilité.

Pour bien comprendre, les valeurs de largeur et hauteur en pourcentage, vous devez savoir d'abord quelques informations.

- L’élément racine HTML et body prennent les dimensions de façon automatique selon la taille de la fenêtre et le contenu de leurs enfants. 
- il prennent 100 % de largeur et l’hauteur suffisante pour afficher le contenue de ses fils et non 100% de l’hauteur de la fenêtre.
- Les valeurs des deux propriété width et height ne sont pas héritées entre le père et ses fils.

Nous commençons par tester l'utilisation d’une valeur en pourcentage avec la propriété largeur.

nous pouvons luis attribué la valeur 100%, dans ce cas,  il  prendra la valeur 600 pixels  qui est égale à  la valeur 100 % de l'élément body 

Si on diminue la valeur à 50 % dans ce cas il va prendre la valeur 300 pixel qui représente 50 % de largeur  de l'élément body. 

Maintenant sinon modifiant la hauteur de paragraphe, et nous lui attribuons la valeur 50%.
Nous voyons qu'il n'y a aucun effet sur l'affichage.

Parce que l’hauteur de l’élément HTML et Body sont déjà été déterminé automatiquement selon le contenue de leurs fils dont notre paragraphe fait partie, dans ce cas la valeur pourcentage de la propriété height ne fonctionnera pas, 

Mais, si nous donne une valeur fixe à body, la valeur en pourcentage fonctionnera, 
Dans notre exemple, nous pouvons donner la valeur 100% de hauteur à l’élément HTML.

Si nous voudront travailler avec l'hauteur nous devons préciser d'abord sa valeur où donner 100 % à l'élémebt  HTML, dans ce cas il prend la valeur 753 px qu’est égale à la hauteur de l’espace afficher dans le navigateur.

Nous devons, aussi, fixer l’hauteur de l’élément body, on peut lui attribuer la valeur 100%, dans ce cas il va prendre la valeur 753px.

Voilà, maintenant, nous pouvons fixer la hauteur du paragraphe en pourcentage.


