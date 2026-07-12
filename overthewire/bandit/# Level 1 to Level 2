## Objectif
Retrouver le mot de passe permettant d'accéder au niveau 2. Le mot de passe se trouve dans un fichier nommé "-" situé dans le dossier "home" de l'utilisateur.

## Ce que j'ai fait
- Après m'être connecté au serveur avec la commande `ssh -p 2220 bandit1@bandit.labs.overthewire.org`
- J'ai utilisé la commande `ls` pour afficher les fichiers présents dans le répertoire. J'ai obtenu un fichier nommé "-".
- J'ai ensuite essayé plusieurs fois de lire son contenu avec `cat -` mais cela ne fonctionnait pas.
- Après quelques recherches, j'ai compris que "-" est interprété par `cat` comme une option et non comme un nom de fichier.
- J'ai donc utilisé `cat ./-` ce qui m'a permis de lire le contenu du fichier et de récupérer le mot de passe du niveau suivant.

## Ce que j'ai appris
J'ai appris que certains noms de fichiers, comme "-", peuvent être interprétés comme des options par les commandes Linux. En ajoutant "./" devant le nom du fichier, on indique à Linux qu'il s'agit bien d'un fichier situé dans le répertoire courant.
