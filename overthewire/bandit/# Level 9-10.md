
## Objectif
Retrouver le mot de passe du niveau 10, stocké dans le fichier `data.txt`, dans l'une des quelques chaînes lisibles par l'homme, précédée de plusieurs caractères `=`.

## Ce que j'ai fait
- Après m'être connecté au serveur avec la commande `ssh -p 2220 bandit9@bandit.labs.overthewire.org`
- J'ai utilisé la commande `ls` pour afficher les fichiers présents dans le répertoire. J'ai ainsi trouvé le fichier `data.txt`.
- J'ai d'abord utilisé `grep "=" data.txt`, j'ai obtenu une erreur indiquant que le fichier `data.txt` est binaire.
- Alors j'ai ajouté `-a` à la commande : `grep -a "=" data.txt`, pour forcer `grep` à traiter le fichier binaire comme un fichier texte. J'ai ainsi pu obtenir la ligne possédant plusieurs `=` et donc le mot de passe du niveau 10.

## Ce que j'ai appris
- Utiliser `-a` pour forcer `grep` à lire les fichiers binaires.
- Un fichier peut contenir des données non lisibles directement, mais aussi des chaînes de caractères exploitables avec les bons outils.

