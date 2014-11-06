#Super boggle
Le boggle est un jeu de société dans lequel il faut retrouver des mots dans une grille de lettres. 
Mais les lettres constituant ces mots ne sont pas forcément alignées, et peuvent serpenter à travers la grille. 
Elles doivent simplement se toucher, à gauche, à droite, en haut, en bas, ou en diagonale.

Par exemple, voici une grille :
```
M A V W  
U S E A  
F I R L  
E O S H
```

On y trouve le mot “SUIS”
```
. . . .  
U S . .  
. I . .  
. . S .
```

ou encore le mot “LAVAS”
```
. A V .  
. S . A  
. . . L  
. . . .
```

###But
Le but de cet exercice est d’écrire un programme qui vérifie si un mot est présent dans une grille, à la façon du 
boggle, mais dans des grilles de taille variable.

###Input
Les données d’entrée sont structurées de la façon suivante :
1. Deux entiers correspondants respectivement au nombre de lignes et au nombre de colonnes de la grille
2. Plusieurs chaines de caractères représentants les différentes lignes de la grille. Attention, il est possible que le nombre de caractère dans la chaine ne corresponde pas au nombre de colonnes annoncés !
3. Des chaines de caractères indiquant les mots à retrouver dans la grille.
4. Le caractère « * » pour indiquer la fin des données d’entrée.

###Output
En sortie, il faudra retourner vrai ou faux pour chaque mot indiqué en entrée, en fonction de la présence ou non du 
mot dans la grille. Si la grille est erronée, il faudra retourner la chaine de caractère « Mauvais format »

###Exemple 1
####Input
4 4 

MAVW 

USEA
 
FIRL
 
EOSH
 
SUIS
 
SOIREE
 
LAVAS
 
*

####Output
true 

false
 
true

###Exemple 2
####Input
5 5 

AIOJS
 
OGNS
 
UELIO
 
ETMLA
 
VPOHA
 
GENS
 
MEGOT
 
GOUT
 
*

####Output
Mauvais format

(Il manque un caractère à la 2e ligne, la grille est donc erronée !)