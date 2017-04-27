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
