TP Formation Git
================

### 0. Configurer Git
``` bash
git config --global push.default simple
git config --global user.email moi@eleves.enpc.fr
git config --global user.name "Prénom Nom"
```

### 1. Cloner le dépôt
``` bash
# Retourner dans son répertoire utilisateur
cd ~
# Cloner le dépot d'exemple
https://github.com/KIClubinfo/formation-git-exemple.git
# Aller dans le dossier
cd formation-git-exemple
```

### 2. Ajouter un fichier
``` bash
# Créer un nouveau fichier, par exemple
echo "Earth's Moon" >> locations.txt
# Git est conscient qu'un nouveau fichier a été créé
git status
# Dire à Git de suivre le nouveau fichier locations.txt
git add locations.txt
```

![Ajouter un fichier](https://www.atlassian.com/dam/jcr:dbf0c59f-848d-4814-bfd5-6b190a092963/03.svg)


``` bash
# Comparer. Le fichier a été ajouté à la staging area et est prêt à être commité
git status
# Commiter le fichier
git commit -m 'Initial commit'
```

![Commiter](https://www.atlassian.com/dam/jcr:d5f60ca0-b606-4e7c-b3a2-430165bc0672/04.svg)

Jusqu'à présent, tout ce que vous avez fait est sur votre système local et invisible pour les autres jusqu'à ce que vous poussiez ces modifications.

``` bash
# Pousser le nouveau commit
git push
```

Vous n'avez pas la permission d'écrire sur le dépôt du TP, vous aurez donc un message d'erreur.