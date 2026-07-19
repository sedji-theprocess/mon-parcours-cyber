
## Objectif
Retrouver le mot de passe du niveau 9, stocké dans le fichier `data.txt`. Il correspond à la seule ligne de texte qui apparaît une seule fois.

## Ce que j'ai fait
- Après m'être connecté au serveur avec la commande `ssh -p 2220 bandit8@bandit.labs.overthewire.org`
- J'ai utilisé la commande `ls` pour afficher les fichiers présents dans le répertoire. J'ai ainsi trouvé le fichier `data.txt`.
- Ensuite, j'ai exécuté la commande `sort data.txt | uniq -u`, pour trier le contenu du fichier grâce à `sort`, puis afficher la ligne qui apparaît une seule fois grâce à `uniq -u`. J'ai ainsi obtenu en sortie le mot de passe du niveau suivant.

## Ce que j'ai appris
- Utiliser `sort` pour trier les lignes d'un fichier.
- Utiliser `uniq -u` pour afficher uniquement les lignes uniques d'un fichier trié.
- Combiner plusieurs commandes à l'aide d'un pipe (`|`) afin d'utiliser la sortie de l'une comme entrée de l'autre.

