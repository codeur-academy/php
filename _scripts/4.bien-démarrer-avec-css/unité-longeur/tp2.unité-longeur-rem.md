# TP 2 - unité longeur rem

Dans ce travail pratique nous allons apprendre à utiliser les unités relative em et racine em.
et comprendre la différence entre eux. 

Pour réaliser ce travail pratique vous avons besoin d'un seul fichier HTML avec le code source de notre article d'exemple.

Par défaut, la valeur de font-size de  l'élément h1 égale 2em, qui signifié la valeur de son père multiplier par 2. Dans notre cas, l’élément body hérite la valeur, par défaut, 16px de l’élément html. donc la propriété font-size de l’élément h1 prend la vlaeur 32px.

Si on lui attribue la valeur à 1em, et 20px à son père body, dans ce cas le font-size de l’élément h1 va prendre la valeur 20px.

Mais si nous attribuons la valeur 20 pixels aliments body automatiquement la propriété de l'élément achat va prendre la valeur 20 pixels.

Si, on change 1em vers 2em, dans ce cas il va prendre 40px.
donc, on comprend très bien, que l’unité **em** multiplie la valeur avec la valeur du père de l’élément.

Maintenant, nous allons voir comment ça marche l'unité racine rem.

Pour un peu de clarté, je vous propose de préciser la valeur la propriété font-size à la valeur  16px.

Si nous attribuer la valeur 1em à l’élément body, la valeur font-size de l’élément h1 prend 32px qui est le double de la valeur de body.

Si nous changeons la valeur de body à 20px, automatiquement h1 prend la valeur 40px.

Dans ce cas, nous voulons que h1 suivre la valeur de l’élément racine HTML et non son père body, nous devons utiliser l’unité rem.

Dans ce cas, la valeur de la propriété font-size de l’élément h1 prend 32px qu’est le double de 16px : la valeur possédée par l’élément HTML.
