# Jeux du Puissance 4
*******************

## Arnaud VILAS BOAS
### DEV8

*******************

### Règle du puissance 4 :

Aligner 4 jetons a la suite(vertical, horizontalement, en diagonale) avant l'adversaire.
Jeux tour a tour.

*******************
Développer en Javascript sans framework

*******************

Le jeu permet de joueur contre un autre joueur ou contre l'ordinateur.
Les scores et le nom des joueur est stocker en localStorage
On peut recommencer une partie
Pour jouer un jeton il suffit de cliquer sur n'importe quel colonne.

Concernant l'IA (partie la plus compliquer).
La première chose qu'il fait:
regarder si le joueur a déjà placer 3 jetons verticalement ou horizontalement et qu'il risque de placer un quatrième ce qui lui permettrai de gagner la partie. Si c'est le cas on place le jeton de l'ordinateur a la suite ou entre les jetons si cela est horizontalement.
Pour essayer de gagner une partie, l'ordinateur va toujours regarder si il peut placer 4 jetons de suite horizontalement ou verticalement.
Il va parcourir le tableau pour trouvé l'emplacement qui lui permettrai de gagner. Il ne place pas de jetons au hazard.
Mais la priorité sera toujours la défense.

Bug connu.
Si l'ordinateur détecte a la deuxième ligne par exemple un emplacement qui lui permet de mettre 4 jetons de suite.Mais qu'a la première ligne il y a une case vide,ce qui fait que le jeton prévu a la deuxième ligne passe sur la première ligne.


*******************
## Avis de Dinh

Première utilisation :

Partie contre IA : trop facile ? j'ai gagné en 4 coups CD capture 1
L'IA est un peu prévisible
Sur le board de la partie contre L'IA, manque le lien pour le menu
au cas où si une personne veut jouer avec moi. de même pour le joueur contre joueur.


Partie joueur contre joueur :

Il serait plus agréable de savoir a qui est le tour.

Pour les noms des joueurs : Il serait bien de proposer une liste de joueur ayant déjà joué a l'application. C'est un peu chiant de retaper son nom à chaque fois. Mais en soi c'est pas très gênant si on veut faire une petite partie.


Expérience utilisateur :

Design classique.
  Un titre parlant mais qui manque de classe.
Utilisation des alert JS un peu abusif.

Commentaire dev :
Fichier bien commenté
fichier tout en un !
les noms des joueur sont sauvegarder dans des localStorages, on pourrait en faire une utilisation plus conséquentes.
Code agréable a lire.

Code ligne 420 et 459 : if repeté deux fois ? possibilité de faire une fonction avec un paramètre différent

Conclusion :

Un puissance 4 fonctionnelle ! Manque juste du style et une IA un peu plus corsée.
