# Utiliser SASS
#### Présentation Ludo

## Mise en place de l'environnement

### 1. Installer RUGBY puis KOALA. 
SASS a besoin d'être complié. La compilation est la traduction d'un fichier écrit par le developpeur en un fichier qui sera interprétable par l'ordinateur. En l'occurance le fichier SASS sera converti ("complié") en fichiers CSS qui seront interprétables par les browsers. Ici la compilation est faite en RUGBY.

Si on ne met pas KOALA on doit faire des lignes de codes en RUGBY pour complier le fichier.

### 2. Organiser ses dossiers/fichiers. 
Il est important de bien organiser ses fichiers puisque KOALA va 'convertir' (compiler) le fichier SASS dans des fichiers CSS. Bonne pratique de Ludo: créer un dossier "assets" dans lequel il y a un dossier CSS et un dossier SASS.

La première chose à faire est de créer un fichier .scss dans le dossier SASS et dans lequel on va écrire le SASS.

### 3. Compilation par KOALA. 
On va ensuite dans KOALA, on glisse le dossier SASS dans les dossiers à traiter.

La première fois il faudra sélectionner le fichier .scss et cliquer sur "compile". Par la suite la compilation sera automatique à chaque modification du fichier .scss

Lors de la compilation, KOALA crée un fichier style.css et un fichier style.css.map (qui reprend la cartographie du fichier SASS et est utile pour le débug; l'inspecteur peut comme ça identifier la ligne source d'une propriété dans le fichier .sass).

Quand on enregistre ensuite le fichier .scss après une modification, KOALA crée automatiquement les fichiers .css correspondant dans le dossier CSS. 

Attention à ne jamais écrire dans le fichier .css qui a été généré puisqu'il sera écrasé par KOALA à chaque nouvelle compilation.

## Intérêt du SASS
SASS permet d'ajouter la notion de programmation dans le CSS. Mais le navigateur ne connait que 3 languagues: HTML, CSS et JS. D'où le besoin de compilation.

Grâce à SASS, les fichiers CSS sont d'avantages réutilisables, mieux organisés, et demandent moins de répétition pour leur création. On peut utiliser des variables, des fonctions,...

Ex: Sur Facebook, tout est blanc sur fond bleu avec de bords gris. Les règles CSS sont réutilisables et permettent d'assurer une cohérence à travers le site. En cas de changement de couleur par exemple, il suffit de changer une variable dans son fichier SASS et non plus de mettre à jour de dizaines de propriétés différentes dans ses fichiers CSS.
