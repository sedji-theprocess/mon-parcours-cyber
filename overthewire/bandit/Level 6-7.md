
## Objectif
Retrouver le mot de passe du niveau 7, qui est stocké quelque part sur le serveur et possède les propriétés suivantes : owned by user bandit7, owned by group bandit6, 33 bytes in size.

## Ce que j'ai fait
- Après m'être connecté au serveur avec la commande `ssh -p 2220 bandit6@bandit.labs.overthewire.org`
- J'ai d'abord utilisé la commande `ls`, mais aucune sortie : le répertoire était vide.
- Ensuite, j'ai utilisé `find / -user bandit7 -group bandit6 -size 33c` pour localiser le mot de passe. J'ai obtenu plusieurs erreurs de type « Permission denied ».
- Après des recherches, j'ai appris qu'il fallait faire suivre la commande `find` de `2>/dev/null` pour nettoyer ces erreurs.
- J'ai donc utilisé `find / -user bandit7 -group bandit6 -size 33c 2>/dev/null`, ce qui m'a donné en sortie `/var/lib/dpkg/info/bandit7.password`.
- Pour finir, j'ai lu ce fichier pour récupérer le mot de passe du niveau 7.

## Ce que j'ai appris
Utiliser la commande `find` suivie de l'utilisateur, du groupe et de la taille. Ajouter `2>/dev/null` à la suite de `find` pour nettoyer les erreurs de type « Permission denied ».

