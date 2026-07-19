
## Objectif
Retrouver le mot de passe du niveau 8, stocké dans le fichier `data.txt`, à côté du mot « millionth ».

## Ce que j'ai fait
- Après m'être connecté au serveur avec la commande `ssh -p 2220 bandit7@bandit.labs.overthewire.org`
- J'ai d'abord utilisé la commande `ls` pour afficher les fichiers présents dans le répertoire, j'ai obtenu le fichier `data.txt`.
- Ensuite, j'ai utilisé `grep "millionth" data.txt` pour rechercher dans le fichier la ligne contenant « millionth » et ainsi récupérer mon mot de passe.

## Ce que j'ai appris
Utiliser la commande `grep` pour rechercher dans le contenu d'un fichier.

