# TP : display block in line

Dans ce travail pratique nous allons 
découvrir les styles par défaut d'un élément HTML
Apprendre la différence entre un élément block,inline et inline-block
Nous terminons par la découverte de comment utiliser la documentation.

Dans ce TP,  nous avons besoin seulement d'un fichier HTML.

Je vous propose de l’enregistrer dans notre espace de travail.

Tout d’abord, nous ajoutons la structure d'un document HTML, ensuite nous insérons le code HTML de notre article d'exemple.

Vous pouvez modifier le titre de la page en  : TP display block inline.

Avant de commencer notre exemple, je vous propose de découvrir les styles par défaut des éléments HTML.

 pour faire nous pouvons utiliser l'outil **inspecter** disponible par défaut dans notre navigateur. Il nous permet de voir le code HTML et les règles de style CSS appliquées à chaque élément de notre page.

Par exemple, ici, l'élément racine HTML s’affiche avec la propriété Display égale **block**.

L'élément **HEAD** lui a été appliqué la propriété **Display** avec la valeur **none**. qui dit au navigateur de ne pas afficher cet élément. 

Et tous les éléments qui lui appartient sont avec la valeur **none** de la propriété **display** .

L’élément **Body** possède  deux propriétés par défaut : 
display en bloc 
et marge égale 8 pixels. 

Dans ce TP, on s’intéresse à la propriété **Display**,  je ne vais pas expliquer en détaille les autres propriétés css par défaut, car nous les découvrirons dans les prochaines sessions de formations.

La balise h1 s’affiche avec display block
La balise p s’affiche aussi display block

Maintenant, commençons notre exemple pratique pour voir comment changer la valeur par défaut de la propriété **Display**. 

Par exemple, nous pouvons commencer par l'élément H1. Il s’affiche par défaut en disposition **Bloc**,  on peut lui donner la valeur **inline** pour  la propriété **display**.. 

On enregistre et on affiche.

on voit pas une grande différence, pourquoi ? 
parce que, c’est vrais,  la disposition **inline**  n'ajoute pas une retour à la ligne, 
mais l'élément suivant paragraphe est en disposition par défaut bloc. ce qui veut dir qu’il ajoute une retourne à la ligne avant et après le paragraphe. 

 pour voir une différence nous pouvons changer la disposition par défaut de paragraphe en valeur inline 

On enregistre et on affiche

 voilà les deux éléments H1 et P sont à disposition **inline**. c’est à dir, il n’ajoute pas une retourne  à la ligne avant et après l'élément.

 Autre chose, avec l'élément inline, on ne  peut pas changer la propriété hauteur et largeur.

Pour test ça, je vous propose de changer la couleur d'arrière-plan de l'élément P pour que vous voyez clairement l’affichage de l’élémént sur le navigateur. 

Pour modifier la propriété largueur, nous utilisons la propriété **width**
et pour modifier la propriété hauteur nous utilisons la propriété **height**

On enregistre et on affiche 

Voilà le changement de la propriété width n’a pas d’effet sur l'affichage de l’élément l’élément inline.

 si nous voulons garder la disposition **inline** et travailler avec les propriétés largeur et hauteur nous devrons utiliser la disposition en inline-block

On enregistre et on affiche 

mais pour voir la modification, nous devons avoir plus d’espace d’affichage sur notre page.

On peut tout simplement agrandir la taille de la fenêtre. 

Voilà les deux éléments H1 et P d’affiche en disposition inline, 
et le  paragraphe s’affiche avec largeur et hauteur puisqu’il est en disposition inline-bloc.

Si vous voulez un autre exemple, vous pouvez changer la propriété width de l'élément a

Mais après l'enregistrement et l’affichage, 

il s’affiche sans le largeur 100 pixels

 pour que le navigateur applique cette propriété vous devez changer la disposition par défaut de l'élément inline vers inline-block

Maintenant je vais vous montrer comment chercher la documentation d’une propriété CSS que vous ne connaissez pas 

par exemple je vais utiliser,  ici,  la propriété **texte-aline** avec la valeur **center** 

Si vous ne connaissez pas cette propriété, vous pouvez chercher sa documentation dans le site web : mo zilla developer network

  
Pour faire il suffit de chercher sur le moteur de recherche Google : text-align MDN 

Où chercher directement dans le site developer.mozilla.org 
et vous trouvez la page de documentation 

La documentation est très utile pour le développeur
 Il lui donne la définition de la propriété et la description de chaque valeur possible.

par exemple ici texte-aline possède  4 valeurs possibles 
stars 
end 
Center 
et justifie 


Maintenant si on utilise l'outil inspecter Nous pouvons voir les règles CSS que nous avons appliqué à l’élément H1 et paragraphe.

Vous pouvez modifier directement les règles CSS dans l'outil inspecter.
vous pouvez activer ou désactiver la règle CSS. 
juste pour voir le résultat d’application dans le navigateur 
mais bien sûr il ne sera pas enregistré dans votre fichier de code dans votre éditeur.

Par exemple pour le paragraphe, nous avons appliqué 4 règles 
background-color 
display : 
Largeur 
et hauteur 

Et pour l’élément **a** nous avons appliqué trois règles 
display inline-block 
text-align Center
et largueur = 100 pixels 
