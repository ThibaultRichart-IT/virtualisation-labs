# TP 3 - Gestion des droits

## Présentation

Ce laboratoire a pour objectif de prendre en main l'environnement Linux et ses commandes de bases.

## Objectifs

*  Comprendre et manipuler les droits d'accès aux fichiers
* Utiliser les commandes chmod, chown, chgrp et sudo.

## Déroulement du laboratoire


### Étape 1 Création d'un environnement de test : 


Sous-étape 1 : Créez un dossier TP2_permissions : 

 <img width="900" height="136" alt="image" src="https://github.com/user-attachments/assets/d65bcf4a-777a-444e-827e-662e71edf1b5" />

1. mkdir TP2_permissions : Créez un dossier TP2_permissions
2. ls : permet de vérifier si le dossier est bien créer, ici c'est le cas.
3. Dans ce dossier, créez un fichier script.sh qui contient '#!/bin/bash' et echo "Test de permission sous Linux"

Sous-etape 2 : Essayez d'executer le fichier script.sh

<img width="706" height="113" alt="image" src="https://github.com/user-attachments/assets/dd10aa2b-8ddc-4771-a10e-58ccfec920de" />

1. Je remarque que je n'ai pas les permissions pour accéder au contenue de ce fichier script.sh


### Étape 2 Modification des droits : 

<img width="780" height="372" alt="image" src="https://github.com/user-attachments/assets/5998a78e-5e40-4658-b4a5-645e799881f9" />

1. chmod u+x script.sh : Donne le droit a l'execution aux utilisateurs pour script.sh
2. ls -l : Vérifier les droits : Je vois le 'r' qui a été ajouté dans la partie utilisateur
3. ./script.sh  : Quand j'éxecute a nouveau, je peux maintenant lire le script.sh car les droits read ont étaient attribué.
4. J'ai maintenant les droits pour ce fichier.

### Étape 3 Expérimentation  :

<img width="849" height="272" alt="image" src="https://github.com/user-attachments/assets/b907d7eb-9748-4678-94d0-c25e851a41ed" />

1. chmod g-r script.sh : Je retire l'accès au 'read' pour le groupe
2. ls -l : Confirme que je viens de retirer le 'read' pour le groupe, j'observe que -rwxrw-r-- deviens rws-w-r-- .
3. J'ai retirer l'accès au 'read' pour le groupe.

Sous étape 3 : Changez le propriétaire du fichier : 

<img width="880" height="192" alt="image" src="https://github.com/user-attachments/assets/d753587b-b451-4061-95d9-fcc8935d9e05" />

1. sudo chown root script.sh : Change le propriétaire du fichier 'thibault' en root
2. ls -l : Permet de vérifier que le propriétaire du fichier à changer en 'root'
3. Le propriétaire est passer de 'thibault' en 'root'

Sous étape 4 : Utilisation de sudo ! 

<img width="900" height="1013" alt="image" src="https://github.com/user-attachments/assets/a62d23b5-13b6-4c93-b6aa-07373556d34f" />

1. ls sudoers : Liste et vérifie la présence du fichier 'sudoers' dans le répertoire courant /etc
2. cat sudoers : Tente d'afficher le contenu du fichier texte 'sudoers' dans le termial avec les droits de l'utilisateur standard (thibault)
3. sudo cat sudoers : Execute la même commande précédente mais en utilisant les privilèges du superutilisateur (root)
4. La restriction d'accès est contournée, j'ai maintenant accès a ce fichier, grace a la commande sudo.

### Conclusion : 

Si je ne me donne pas les permissions, l'accès ne m'est pas autourisées, en revanche une fois les autorisations rwx effectué, je peux travailler sur la fiche.


### Fin de TP3
