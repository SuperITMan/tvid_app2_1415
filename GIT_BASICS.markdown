# Tutoriel Git & Github

## Installation
Je présume que vous travaillez sous Windows, si pas vous savez certainement mieux que moi comment installer des paquets sur votre \*NIX.
Pour commencer pas de SourceTree ou autre crapulerie, Git fournit un programme formidable que vous pourrez vous procurer ici :  
[http://git-scm.com/downloads]  
Installez-le tout en gardant les paramètres par défaut.

## Initialisation
Une fois installé, lors d'un clic droit daes votre espace de travail, le menu contextuel doit vous présenter les options suivantes :  

L'option Git Bash vous fera apparaître une console Git positionnée à l'endroit où vous avez lancé ce Bash.  
(Vous pouvez utiliser "cd" pour naviguer dans l'arborescence.)   

Avant toute chose il faut configurer Git avec votre identité, entrez les commandes suivantes : 

    git config --global user.name "John McKek"
	git config --global user.email johnkek@example.com

![alt text](https://github.com/srozen/tvid_app2_1415/blob/work_srozen/images/gitconfig.PNG)

Positionnez-vous dans un dossier qui va accueillir le dossier du projet, "Documents" par exemple.  

Pour récupèrer le projet, il faut le cloner dans votre espace personnel avec la commande:   

    git clone https://github.com/srozen/tvid_app2_1415

![alt_text](https://github.com/srozen/tvid_app2_1415/blob/work_srozen/images/gitclone.PNG)

Vous voilà avec le repo dans votre espace personnel !

## Master et les branches

Master est la branche principale qui recueillera les changements collectifs
et celle sur laquelle vous devrez vous mettre à jour.   

Lancez un git bash dans le dossier __tvid_app2_1415__ .   
Maintenant, votre prompt vous dis normalement que vous êtes sur Master.   

Pour savoir sur quelle branche vous êtes:

    git branch

Pourchanger de branche et vous déplacer sur Master (Le tronc commun), faites :   
    
	git checkout master

Ensuite, pour télécharger la toute dernière version de Master :   
    
	git pull

![alt_text](https://github.com/srozen/tvid_app2_1415/blob/work_srozen/images/gitupdate.PNG)

## Créer votre branche et travailler dessus
## Soumettre votre travail
--------------------------
## Cycle de fonctionnement
1. `git checkout master` Pour vous positionner sur Master
2. `git pull` Pour intégrer les changements sur Master
3. `git checkout votre_branche` Pour revenir sur votre branche
4. `git merge master` Pour transposer les changements de Master sur votre
branche et donc vous mettre à jour.
5. *Vous effectuez votre travail (**Sur votre branche !**)*...
6. `git status` Une fois que vous avez terminé pour voir où vous en êtes.
7. `git add new_file` Si vous avez créé un nouveau fichier à envoyer
8. `git commit -am "votre_msg_de_commit"` Pour commit tout les fichiers
inclus et modifiés (-a) avec un message (-m).
9. `git push origin votre_branche` Pour envoyer votre travail en ligne.
