# Navy
Projet 1ère année Epitech module PSU

Le Navy a pour but de reproduire le jeu Bataille Navale entre deux processus grâce aux signaux.

Projet mis à la norme d'Epitech, passant 100% des tests.

<br>Communication par décalage de bit, checksum et ping-pong.

Compilation par Makefile. (make all)

#

Exemple de map dans le fichier pos.

Usage:
<br>./navy [pid] map

Exemple:
<br>./navy pos
<br>./navy 3241 pos
  
#

Projet mis à titre d'exemple pour vous aider a vous inspirer.
<br>Copier le projet tel quel est inutile pour progresser.

<br>Développé par Bastien Rinck et Thibaut Cornolti.

#

## Example

### Premier navy

```
my_pid: 31567
waiting for enemy connexion...
enemy connected

my positions:
 |A B C D E F G H
-+---------------
1|. . 2 . . . . .
2|. . 2 . . . . .
3|. . . . . . . .
4|. . . 3 3 3 . .
5|. 4 . . . . . .
6|. 4 . . . . . .
7|. 4 . 5 5 5 5 5
8|. 4 . . . . . .

enemy's positions:
 |A B C D E F G H
-+---------------
1|. . . . . . . .
2|. . . . . . . .
3|. . . . . . . .
4|. . . . . . . .
5|. . . . . . . .
6|. . . . . . . .
7|. . . . . . . .
8|. . . . . . . .

attack: C1
C1: missed

waiting for enemy's attack...
C1: hit

my positions:
 |A B C D E F G H
-+---------------
1|. . x . . . . .
2|. . 2 . . . . .
3|. . . . . . . .
4|. . . 3 3 3 . .
5|. 4 . . . . . .
6|. 4 . . . . . .
7|. 4 . 5 5 5 5 5
8|. 4 . . . . . .

enemy's positions:
 |A B C D E F G H
-+---------------
1|. . o . . . . .
2|. . . . . . . .
3|. . . . . . . .
4|. . . . . . . .
5|. . . . . . . .
6|. . . . . . . .
7|. . . . . . . .
8|. . . . . . . .

attack: 
[...]
```

### Second navy

```
my_pid: 31587
successfully connected

my positions:
 |A B C D E F G H
-+---------------
1|. . . 2 . . . .
2|. . . 2 . . . .
3|. . . . . . . .
4|3 3 3 . . . . .
5|. 4 . . . . . .
6|. 4 . . . . . .
7|. 4 . 5 5 5 5 5
8|. 4 . . . . . .

enemy's positions:
 |A B C D E F G H
-+---------------
1|. . . . . . . .
2|. . . . . . . .
3|. . . . . . . .
4|. . . . . . . .
5|. . . . . . . .
6|. . . . . . . .
7|. . . . . . . .
8|. . . . . . . .

waiting for enemy's attack...
C1: missed

attack: C1
C1: hit

my positions:
 |A B C D E F G H
-+---------------
1|. . o 2 . . . .
2|. . . 2 . . . .
3|. . . . . . . .
4|3 3 3 . . . . .
5|. 4 . . . . . .
6|. 4 . . . . . .
7|. 4 . 5 5 5 5 5
8|. 4 . . . . . .

enemy's positions:
 |A B C D E F G H
-+---------------
1|. . x . . . . .
2|. . . . . . . .
3|. . . . . . . .
4|. . . . . . . .
5|. . . . . . . .
6|. . . . . . . .
7|. . . . . . . .
8|. . . . . . . .

waiting for enemy's attack...
[...]
```
