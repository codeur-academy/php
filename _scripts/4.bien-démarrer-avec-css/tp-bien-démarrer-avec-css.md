# TP : bien-démarrer-avec-css


## Structuration de texte en HTML

Dans ce travail pratique nous avons besoin d'un dossier de travail qui va contenir 
des fichiers CSS
des images 
et un fichier html

Je vous conseille d'enregistrer ce dossier dans votre espace de travail.

Tout d'abord nous commençons notre travail pratique par la création d'un dossier nommé **CSS** qui va contenir les fichiers CSS externes que nous allons créer pendant notre travail pratique.

 nous avons besoin aussi d'un fichier HTML nommé **index.html** qui va contenir le contenu structuré de notre article.

Nous insérons d'abord la structure d’une page HTML valide.

Dans la l’élément titre, nous pouvons écrire le titre **Qu'est-ce que l'ordinateur**.

Pour insérer nos règles CSS sur la page HTML, je vous propose toujours d’utiliser un fichier css externe, ça vous permet de bien organiser vos règles afin de les utiliser sur plusieurs page web de votre projet, par conséquent ça va vous faciliter la maintenance de votre code CSS.

Maintenant, pour relier le fichier CSS à notre page, nous utilisons la balise link dont l’attribut href égale le chemin correct de notre fichier css.


Ensuite, nous allons créer la structure de notre page d'articles

Généralement une page web peut-être structuré en deux parties :
 la première partie appelée **main** qui va contenir tout le contenu de notre article 
et la deuxième partie s'appelle **footer** qui va contenir le pied de page

 normalement la balise main peut contenir plusieurs sections, dans notre cas, nous avons besoin qu’un seul section qu’on peut l'identifier par la tribu **id**  :  **page-container**.

Sur l’élément section, nous pouvons ajouter l'élément article qui représente un article sur la page.

L’article peut être structuré en trois parties :
Tout d'abord l'élément header  qui va contenir le titre de l'article et ces catégories
La deuxième élément figure, qui peut présenter l’image de l’article.
et la troisième élément qui va contenir le contenu de l'article, qu'on peut l'associer à la classe **content**  pour le bien cibler par les sélecteurs CSS.

Avant de continuer notre travail pratique je vous propose d'installer l'extension **live server** qui vous permet d’actualiser la page sur le navigateur à  chaque modification des fichiers HTML ou CSS.

Comme ça à chaque modification vous pouvez voir l'affichage sur le navigateur en temps réel sans actualisation. 
Car, pratiquement en développement, nous utilisons deux écrans,un écran pour l'éditeur de code et un autre écran pour l’affichage du résultat.

Mais dans notre formation puisque nous avons qu'un seul écran, je vais essayer de diviser
l’écran en deux parties.

Maintenant notre structure interne de l'article est terminé, il ne reste qu'à insérer le contenu de l'article.

 Dans l’élément header nous pouvons ajouter le titre de l'article en utilisant l'élément H1.
et la date de modification en utilisant l'élément paragraphe.
Les catégories de l’article peuvent être structurées en utilisant les liens hypertexte.

Dans notre cas, l'article a deux catégories :  informatique et outils.

 Normalement l'attribut href doit contenir le chemin de la page catégorie, mais puisque nous n'avons pas cette page pour le moment, on peut mettre la valeur dièse qui signifie:  lorsqu'on clique sur le lien on reste sur la page actuelle. 

Pour faciliter le ciblage de ces éléments par CSS, nous pouvons associer le paragraphe à la classe **date** et les deux catégories as la classe **category**.


À l'intérieur de l’élément figure, nous pouvons ajouter une image qui représente l'article. 
Pour ce faire, nous avons besoin de créer un dossier nommé images dont lequel nous pouvons déposer notre image d’article qui s'appelle ordinateur.png.

Maintenant pour insérer l'image à document, vous pouvez utiliser l'élément **img** avec le chemin correct. et ne pas oublier d'insérer un texte alternatif où cas, où le navigateur n'a pas réussi à charger l'image.

Dans la section associé à la classe **content**, nous pouvons ajouter le contenu de notre article structuré en HTML.

Il contient :
Un paragraphe avec un lien hypertexte
une liste non ordonnée 
un titre de niveau deux
un paragraphe 
et une liste ordonnée 

## Normalisation des style par défaut entre les navigateurs

Maintenant on va passer à stylisé notre article.
 mais avant de commencer j'aimerais vous expliquer le problème de normalisation des règles css par défaut entre les navigateurs.

 En général chaque élément HTML possède des règles par défaut proposé pour chaque navigateur,  
Le problème est que chaque navigateur spécifie des règles différents de l'autre, ce qui pose un problème d'affichage de résultat final après le travail du développeur css dû à la différence entre les valeurs par défaut de chaque navigateur.

Pour résoudre ce problème les développeurs utilise une bibliothèque qui s'appelle **normalize** qui normalise les règles par défaut des éléments HTML pour tous les navigateurs.

Pour trouver cette bibliothèque vous pouvez utiliser le moteur de recherche Google, avec le mot-clé **normaliz**, il vous dirige directement vers la page principale de la bibliothèque normalize css.

Pour télécharger, vous pouvez cliquer sur télécharger , le navigateur vous redirige directement vers le fichier CSS qui contient tous les règle CSS de la bibliothèque,

 vous pouvez faire un copier-coller et taper vers votre éditeur de code.
C'est mieux de insérer le code dans un nouveau fichier nommée **normalize.css**.

Ensuite en utilisant la balise link, nous pouvons importer les déclarations de normalisation sur notre fichier HTML. 

Maintenant si vous utilisez l'inspecteur de code, vous pouvez détecter les modifications réalisées par la bibliothèque normalize
 Par exemple l'élément H1 a pris la valeur 2em pour la propriété font-size. 
On remarque aussi quelques modifications sur les valeurs des marges.

Ensuite vous pouvez consulter les différents éléments pour voir ce que la bibliothèque normalize à apporter comme modifications sur les valeurs par défaut de chaque élément de notre page.

## Changement d'apparence de notre article

Maintenant après avoir normalisé les valeurs par défaut des différents éléments HTML, nous commençons la modification d'apparence dans notre article.

 c'est mieux de commencer par les balises parents jusqu'aux balises fils. 
nous pouvons commencer par l’élément body 

La première chose à faire, est de préciser le style de font.

Nous pouvons utiliser l'un des style proposé par Visual Studio code, ou chercher dans la bibliothèque Google Fonts. 

Par défaut le site Google font vous propose les fonts les plus utilisés par les développeurs. vous pouvez naviguer cette page, et trouver le bons font à utiliser sur votre article. 

Par exemple nous pouvons utiliser ce style appelé : open sans 

Par défaut le site google font, vous propose la balise link à utiliser dans votre page HTML 

Aussi, il vous propose la déclaration CSS à utiliser dans votre fichier pour bien appliquer ce style de font.

On peut augmenter la distance entre les ligne en utilisant la propriété  **line-height** avec la valeur 1. 5 qui égale à 16px multiplié par 1.5.

L’élément identifier par le Id : **page-contrainer**, englob tous le contenue de notre page, on peut ajouter un peu d’espace entre l’élément et les côtés du navigateur en utilisant la propriété **padding** avec la valeur 3 rem qui est égal à 16 fois 3 pixels.

On peut ajouter un peut d’espace entre l’élément header et le reste de contenue en utilisant la propéité **maring-bottom**.

Aussi, c’est mieux de diminuer l’espace entre le titre et la date de l’article, en utilisant la propriété **maring-bottom**.

Pour la couleur du titre, utilisez la propriété **color** avec la valeur indigo.

Pour la date, on peut initialiser les marges à zéro pixel sauf le marge en bas,  qu'on peut lui attribuer la valeur 4 pixels c’est à dire 0,25 rem.
Nous pouvons changer sa couleur en gris et forme de style en italique.

Pour les catégories, nous pouvons changer la couleur d'arrière-plan en indigo par conséquent nous devons changer aussi la couleur de texte en blanc pour qu'il apparaisse clairement. 

aussi c'est mieux d'enlever  le soulignement en utilisant la propriété text-decoration = non

 On peut ajouter un peu de padding.

 Pour un peu de beauté nous pouvons ajouter la propriété border-radius.

 On peut diminuer un peu la taille des caractères et changer changer l'opacité à 0,75 %.

 passons maintenant à l'affichage de l'image, 

notre image existe à l'intérieur de l’élément figure, nous pouvons ajouter des bordures de 1 pixels et couleur noire.

Pour centrer l'image nous pouvons utiliser la propriété  **texte-aign** avec la valeur Center

-------

 C'est mieux d'ajouter un peu de padding, pour laisser un espace entre l'image et le bordure de l'élément figure. 

Pour un peu de beauté, vous pouvez ajouter border-radius de 0,25 rem.

 à ne pas oublier, d'ajouter un peu d'espace entre l'image et le reste de l’article en utilisant la propriété **margin-bottom**.


 Pour le texte de notre articles, nous pouvons augmenter la taille des caractères et ajouter un peu d'espace entre les paragraphes en utilisant la propriété **margin-bottom**.

Je vous propose d'appliquer les mêmes déclarations  sur la liste ordonnée et la liste non ordonnée.

Pour ajouter des styles à l'élément lien hypertexte vous pouvez utiliser le pseudo-class **link** qui nous permet de changer l'apparence des liens qui n'ont pas encore été visités.

Pour changer l'apparence des liens déjà visités, vous pouvez utiliser le pseudo class **visited**. 
comme ça on aura une différence d'affichage entre les liens visités et i ce qui ne sont pas encore visité.

il existe un autre pseudo classe qui s'appelle **hover** qui vous permet d’activer un style css quand on survole sur le lien. on peut changer la propriété text-decoration vers  **underline**.

Nous avons presque terminé. il ne reste qu’à changer l’apparence du pied de page. 

D'abord nous devons ajouter le padding-left  et right pour incliner le paragraphe avec notre contenu.
 ensuite on peut ajouter un peu d'espace interne en utilisant la propriété padding-top et padding-bottom.

Pour que le pied de page soit visible on peut changer sa couleur d'arrière-plan au noir 
et la couleur de texte en blanc

Voilà maintenant, nous avons créé notre première page réelle et professionnelle en utilisant HTML et CSS. 
