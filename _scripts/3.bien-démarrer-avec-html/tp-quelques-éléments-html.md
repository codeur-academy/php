# Script de TP - Quelques éléments  HTML

## Présentation du résultat final

Dans ce travail pratique nous allons réaliser cette page web qui présente à un article nommé :  **qu'est-ce que l'ordinateur**

Tout d'abord il contient 
- le titre de l'article suivi par une image 
- puis une paragraphe suivi par une liste non ordonné.
- Ensuite un titre de niveau 2 suivi par un paragraphe et une liste ordonnée.

## Présentation des documents de départ

Pour réaliser ce travail pratique, je vous ai préparé deux documents 

- un fichier texte contenant tout le texte 
- et une image qui présente le sujet de l'article .

## Réalisation de TP

Tout d'abord nous ouvrons le dossier de travail dans dans notre éditeur de code.

Il contient :
- le fichier texte
- est l'image que nous allons utiliser.

Nous commençons par la création d'un document nommer **index.html**

**Mais, pourquoi ce nom ?**

Parce que, pratiquement dans un **serveur web**, 
la page qui porte ce nom s'affiche **par défaut** 
si l’utilisateur consulte notre dossier par une adresse web 
qui ne préciser par le nom du fichier à consulter.

...

Tout d'abord nous ajoutons la structure d'un document HTML valide,
puis, nous insérant notre texte à l'intérieur de l'élément  body.

avant de commencer notre travail pratique, 
j'aimerais de vous montrer l'affichage de notre texte sans le structurer par HTML 
afin de vous montrer l'intérêt d'utiliser ce langage pour la création des pages web.

Voilà le navigateur affiche tout le texte dans un seul **bloc**, même si que notre texte est un peut organisé au départ. 
par exemple nous avons ajouté 
- des retours à la ligne 
- et des tiret de 6 pour structurer la liste.

L'objectif du HTML est structurer le texte en disant au navigateur que,
- ça c'est un titre 
- et ceci est une image 
- et cela est une liste. 

...

et C'est ce que nous allons réaliser dans ce travail pratique.


Tout d'abord, nous insérons le titre de la page qui s'affichera sur le la zone titre du navigateur. 

Pour le titre de niveau 1 de l'article, nous utilisons l'élément **H1**.

...

à chaque modification je vous montrerai le résultat pour que vous me suivez très bien.

...

Pour insérer une image à notre document nous utilisons l'élément **img** 
qui contient 2 attributs 
- le premier s'appelle **src** pour source
- et le deuxième **alt** pour alternative 

sur l'attribut **source** nous spécifions l'emplacement de l'image 
et sur l'attribut **alt** nous écrivons le texte qui s'afficher si le navigateur n'arrive pas à charger ou trouver l'image sur le serveur.

sur l'attribut **source** nous utilisons notre image **ordinateur.png**.
Notez ici que nous avons juste écrit le nom de l'image sans spécifier le chemin. 
parce que l'image existe dans le même répertoire avec notre document html.

Et sur l'attribut **alt**, nous écrivons le texte **exemple d'un ordinateur**.

Pour bien voir l'utilité de l'attribut **alt**, vous pouvez par exemple changer le nom du chemin de notre image, 
Par exemple ajoutons la lettre s à la fin d'ordinateur.  
comme ça le navigateur nous trouvera pas l'image et affichera le texte alternatif au lieu de l'image.

...

Ensuite pour insérer un paragraphe nous utilisons l'élément **P** 

Pour insérer une liste non ordonnée  nous utilisons l'élément **UL** pour **unordered list** en anglais.

à l'intérieur de **list** nous utilisant l'élément **li** a pour **liste item** en anglais qui représente un élément de la liste.

Nous ajoutons seulement le texte sans les **tiret de 6**. parce que la liste non ordonnée s'affiche par défaut  avec des cercles avant chaque élément de la liste.

Observez dans le résultat, qu'avec HTML nous nous pouvons pas changer l'apparence des éléments, car le navigateur utilise des styles par défaut pour chaque élément HTML.

pour changer cette apparence nous allons voir dans la partie CSS comment utiliser le langage CSS pour changer l'affichage de chaque élément sur le navigateur.

Une chose très important pour le langage HTML, est que l'objectif n'est pas de changer l'apparence de texte mais de 
- structurer le texte 
- et de donner un sens sémantique à chaque partie de notre texte.
  - par exemple on dit que cette parti est un titre de niveau 1
  - est la partie suivant est une paragraphe 
  - et cela est une liste.
  - 
 avec cette façon de faire, nous allons aider les moteurs de recherche à bien comprendre et référencer notre page web sur internet.

Revenons maintenant à notre TP, 
  
pour ajouter le titre de niveau 2  nous utilisons l'élément **H2** 

Ensuite un paragraphe en utilisant l'élément **P** 

Et pour la liste ordonnée nous utilisons l'élément **OL** pour **ordered liste** en anglais.
et à l'intérieur nous utilisons l'élément **li** qui représente un élément de la liste. 

Dans cette fois, nous n'avons pas besoin de ces numéros, parce que ils seront afficher par défaut par le navigateur. 

Et finalement on enregistre et on affiche notre article.

Le titre s'affiche sur la zone titre de l'onglet.
ensuite le contenu que nous avons insérer 
et à la fin la liste ordonnée qui s'affiche avec les numéros.