# TP 1 – Découverte de l’environnement Linux

## Présentation

Ce laboratoire a pour objectif de prendre en main l'environnement Linux et ses commandes de bases.

## Objectifs

*  Se familiariser avec le terminal et la hiérarchie du système Linux
* Utiliser les cmmandes de base pour naviguer, créer et manipuler des fichiers.

## Déroulement du laboratoire


### Étape 1

Manipulation de fichiers : 


Sous-etape 1 : Créez un dossier TP1_Linux dans mon dossier personnel : 

 <img width="706" height="381" alt="image" src="https://github.com/user-attachments/assets/253c9c3d-9178-44f3-a2c5-eeaca93c2773" />

 1. mkdir TP1_Linux : Créer le dossier TP1_Linux
 2. cd TP1_Linux : Rentre dans le dossier précédemment créer.
 3. touch notes.txt && touch todo.txt : Créer deux fichier todo et notes.
 4. ls -l : affiche les deux fichiers, leurs infos et leurs droits.

Sous-etape 2 : Editez le fichier notes.txt avec nano ou echo et entrée une phrase.

<img width="900" height="75" alt="image" src="https://github.com/user-attachments/assets/a64add8b-67da-4f72-9a37-8e0f4678873f" />

echo : Ajoute le texte a mon fichier notes.txt.

Sous-etape 3 : Copiez ce fichier vers back_notes.txt , Renommez todo.txt en taches.txt et supprimez le fichier backup_notes.txt : 


<img width="900" height="167" alt="image" src="https://github.com/user-attachments/assets/516100eb-cc7a-46d4-b2ea-92177c31771c" />

1. cp notes.txt backup_notes.txt : Copie le fichier notes.txt dans un nouveau fichier backup_notes.txt
2. mv todo.txt taches.txt : Rename todo.txt en tache.txt
3. rm backup_notes.txt : Supprime backup_notes.txt de manière irréversible.

## Etape 2 

Recherche et affichage : 

Sous-etape 2 : Affichez le contenu du fichier notes.txt avec cat

<img width="719" height="111" alt="image" src="https://github.com/user-attachments/assets/f5111835-3b24-4cd6-ba48-9aa9aff1d647" />

1. cat notes.txt : Affiche le texte a l'intérieur du fichier notes.txt

Sous etape 2.1 : Recherchez le mot 'Linux' dans le fichier notes avec grep

<img width="753" height="236" alt="image" src="https://github.com/user-attachments/assets/256f2e1c-f8f0-49fc-8bc3-4398edc2f81e" />

1. grep "Linux" notes.txt : Affiche en surbrillance le mot concernés. Rien ne s'affiche si rien n'est as affiché.

Difficulté rencontré : J'ai tout de même du m'y reprendre a plusieurs fois car je n'arriver a mettre dans l'ordre les actions, soucis règler après quelques essais. 

Conclusion : Le dossier TP1_Linux a bien été créer, la créations des deux fichiers.txt ont bien été fais, L’édition d’un fichier a aussi était fait correctement, ainsi la copie dans backup_notes.txt. Les recherche et les affichage  notamment avec cat m’ont permis de bien voir que mon fichier était correctement paramétrer, et pour finir la commande grep m’as bien montré que ‘Linux’ était bien présent dans mon fichier.


## FIN DE LAB
