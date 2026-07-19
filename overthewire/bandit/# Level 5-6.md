# Level 5 to Level 6

## Objectif
Retrouver le mot de passe permettant d'accéder au niveau suivant le niveau 6. Celui-ci est stocké quelque part sous le dossier `inhere` et possède ces caractéristiques : human-readable ; 1033 bytes in size ; not executable.

## Ce que j'ai fait
- Après m'être connecté au serveur avec la commande `ssh -p 2220 bandit5@bandit.labs.overthewire.org`
- J'ai d'abord utilisé la commande `ls` pour afficher les dossiers présents dans le répertoire, j'ai obtenu le dossier `inhere`.
- Ensuite, je suis entré dans ce dossier grâce à `cd`.
- J'ai trouvé une liste de dossiers `maybehere00` à `maybehere11`.
- J'ai utilisé la commande `find . -type f -size 1033c` dans le dossier `inhere` pour ressortir le fichier ayant les caractéristiques demandées. J'ai obtenu comme sortie `./maybehere07/.file2`.
- Enfin, j'ai utilisé `cat ./.file2` pour lire ce fichier et ainsi récupérer le mot de passe.

## Ce que j'ai appris
Utiliser la commande `find` suivie du type et de la taille du fichier recherché pour le localiser.




