#Détecteur de carré

###But
Le but de cet exercice est d’écrire un programme qui détecte des formes géométriques dans une matrice de caractères. 
Ici, on se contentera d’un détecteur de carré.

###Sujet
Il vous sera donné une grille de dimension N x N, chaque cellule contenant soit un « . » (cellule vide), soit un « # »
(cellule pleine). 

Vous devrez indiquer si la grille contient au moins une forme carré plein, c’est-à-dire au moins un sous-ensemble m x m (m <= N) 
de la grille dont toutes les cases sont pleines, mais sans qu’aucune ligne ou colonne ne dépasse du sous-ensemble 
(voir le 5e exemple ci-après). Attention, les cases ne forment pas de sous-ensemble avec d’autres cases qu’elles 
toucheraient en diagonale.

###Exemple

La grille suivante contient un carré :
```
. # # . 
. # # . 
. . . . 
. . . .  
```

Mais ces grilles-ci n’en contiennent pas :
   ```
   . # # . .  
   . # . . .  
   . . . . .  
   . . . . .
   
   . # # . .  
   . . # # .  
   . . . . .  
   . . . . .  
   . . . . .
   
   . # # # .  
   . # . # .  
   . # # # .  
   . . . . .  
   . . . . .
   
   . . . . .  
   # # # . .  
   . # # # .  
   . . . . .  
   . . . . .
   ```
(La figure « déborde » du carré central, et n’est donc pas un vrai carré).

###Input
En entrée, vous recevrez un premier indiquant le nombre de grilles à tester par le programme. 
Ensuite pour chaque grille, vous recevrez un entier indiquant la dimension N de la grille, puis N lignes de N 
caractères correspondant à la ligne.

###Output
En sortie, vous indiquerez pour chaque cas si la grille contient au moins un carré ou non.

###Exemple

####Entrée

4
 
4
```
. # # .  
. # # .  
. . . .  
. . . .
```
5
```
. # # . .  
. # # # .  
. . . . .  
. . . . .  
. . . . .
```
5
```
. # # . .  
. # . . .  
. . . . .  
. # . . .  
. . . . .
```
5
```
. # # # .  
. # . # .  
. # # # .  
. . . . .  
. . . . .
```

####Sortie
Cas 1: OUI 

Cas 2: NON
 
Cas 3: OUI
 
Cas 4 : NON