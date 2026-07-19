## Objectif
Faire ressortir le mot de passe du niveau 3 dans un fichier appelé '--spaces in this filename--' situé dans le dossier "home" de l'utilisateur.

## Ce que j'ai fait
- Après m'être connecté au serveur avec la commande `ssh -p 2220 bandit2@bandit.labs.overthewire.org`
- J'ai utilisé la commande `ls` pour afficher les fichiers présents dans le répertoire. J'ai obtenu un fichier nommé '--spaces in this filename--'.
- Précedemment j'ai pu comprendre l'utilisation de la commande cat avec les fichiers dont les noms possèdent des tirets et des espaces .

- J'ai donc utilisé 'cat  "./--spaces in this filename" ' ce qui m'a permis de lire le contenu du fichier et de récupérer le mot de passe du niveau suivant.

## Ce que j'ai appris
J'ai appris l'utilisation de la syntaxe de la commande cat pour les fichiers dont les noms possèdent des espaces . 
