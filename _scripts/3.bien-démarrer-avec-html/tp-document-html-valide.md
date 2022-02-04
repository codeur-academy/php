https://docs.google.com/document/d/1rkLSqlZBTzIBADS4PQhFM3v_ZuolS4kVeobUDY0mYeo/edit

Dans ce travail pratique nous allons apprendre comment créer un document HTML valide.

Mais, avant de commencer je vous conseille d'enregistrer le document HTML dans votre dossier des travaux pratiques.
Document HTML valide  

Pour créer un document HTML valide, nous devons commencer par l’élément  DocType
qui détermine la version du langage HTML, dans notre cas c’est la version 5.

Ensuite nous ajoutons l'élément racine HTML qui va comprendre tout le contenu de la page.

À l'intérieur nous devons ajouter deux éléments, tout d’abord  l'élément <head>.

ensuite, l’élément body. Pour l'écrire, vous pouvez  juste taper le nom body suivi par tabulation, Visual Studio Code va comprendre directement que vous voulez insérer l'élément body. 

  À l'intérieur de l'élément head  vous devez ajouter la balise meta charset  UTF-8 . 
Qui détermine l’encodage des caractères à utiliser par les navigateurs pour lire le code de votre page web. 
 
Ensuite c'est mieux d'ajouter l’élément Title qui détermine le titre de la page à afficher dans le navigateur est dans le les résultats des  moteurs de recherche comme par exemple google.com. 
 
 remarquez que dans l'élément head toutes les informations que nous avons écrit n'apparaissent pas dans la page web mais c’est balise body qui va contenir  les informations de la page. 
 
À l'intérieur de l'élément Body vous pouvez ajouter le contenu de votre page web par exemple nous pouvons ajouter le paragraphe “Voici ma page web”. 
 
Voilà nous avons créé notre premier document HTML valide, il ne reste qu’enregistrer notre document en utilisant contrôle S. 
 
Ensuite vous pouvez tester votre page, voilà.
 
Notez ici, comment le titre s'affiche dans la zone titre du navigateur les éléments de body s'affiche comme contenue de la page. 
Encodage de la page 
J'aimerais vous ajouter plus d'explications à propos de l'élément meta charset utf-8.
 
Pour bien voir l'effet de déterminer le  codage des caractères,  nous devons ajouter quelques mots contenant  des caractères accentués. 

 Par exemple, dans l’élément titre nous écrivons  :  Ma première page. 
et dans le paragraphe:  voici ma première page web.
 
Maintenant le contenu de la page s'affiche correctement dans le navigateur, pour voir l'intérêt de l’élément meta charset, je vais changer l’encodage, nous allons changer UTF-8 par ASCII .
 
Après l'exécution vous voyez très bien que le caractère français “è” ne s'affiche pas correctement soit dans le titre ou dans le paragraphe. 
 
Mais, ça veut dire quoi à ASCCII. 

C’est un tableau d’encodage qui définit 128 caractères qui peut être utilisé sur Internet et il  comprends les chiffres entre 0 et 9 les lettres anglais de A à Z minuscule et majuscule et quelques caractères spéciaux.

 Ce type d'encodage ne vous permet pas d'afficher les caractères en français. 
Par contre l'encodage UTF-8 vous permet d'afficher presque tous les caractères :de l'anglais, du français et même  d’arabe. 
Utilisation des raccourcis
Il existe une façon très simple pour créer un document HTML valide dans Visual Studio code. 

C’est d’utiliser le raccourci HTML:5 et non HTML . le raccourci HTML ajoute tout simplement la balise HTML par contre le raccourci  HTML:5 vous permet d’ajouter la structure complète d'une page html valide. 

Il parait qu’il vous a ajouté le code avec plus de configuration et  des balistes. 

Par exemple l’attribut lang de l’élément HTML détermine la langue de la page, il détermine la langue compréhensible par les visiteurs probable de votre page web. 

La différence entre cette configuration et la balise meta charset et que la balise meta détermine comment les caractères sont interprétés par le navigateur par contre l’attribut langue détermine la langage des utilisateur cible. 

Dans notre exemple, puisque nous écrivons pour les gents qui comprend le français, nous écrivons “fr”, c’est à dir français.

  Cette balise est utilisée pour adapter l'affichage de la page à l'affichage mobile. je vais pas détailler l'explication ici, car nous allons voir ça après dans une sessions spécifique pour l’affichage des pages sur mobile.


Cet élément permet l’optimisation d’affichage de notre page sur le navigateur Internet Explorer.

Ensuite vous pouvez continuer la saisie de contenu de votre page puis enregistrer.
