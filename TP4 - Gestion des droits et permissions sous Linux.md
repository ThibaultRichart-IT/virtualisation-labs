# TP 4 - Système de fichiers 

## Présentation

Ce laboratoire a pour objectif de prendre en main l'environnement Linux et ses commandes de bases.


## Objectifs

*  Créer dans mon répertoire personnel les fichiers selon l'arborescence suivante :

<img width="802" height="277" alt="image" src="https://github.com/user-attachments/assets/4a0dabde-8e8a-4bf2-8f9c-e9822718a835" />


## Déroulement du laboratoire


### Étape 1

Manipulation de fichiers : 


Sous-etape 1 : Créez deux répertoires Unix et Python dans mon répertoire personnel.

<img width="727" height="227" alt="image" src="https://github.com/user-attachments/assets/873367e7-1be3-4543-8cbc-de2fedb2597c" />

1. mkdir Unix Python : Créer le dossier Unix et Python

Sous Etape 2 : Créer deux répertoires TP1 et TP2 dans le répertoire Unix

<img width="630" height="217" alt="image" src="https://github.com/user-attachments/assets/3fe31675-dd36-4f74-94d6-fb05f22d7f9e" />

1. mkdir TP1 TP2 : Créer un dossier TP1 et TP2 dans le chemin ~/Unix
2. ls : Permet de confirmer que les fichier TP1 et TP2 sont bien créer

Sous Etape 3 : Copier les deux répertoires TP1 et TP2 dans le dossier Python.

<img width="716" height="80" alt="image" src="https://github.com/user-attachments/assets/63fbc304-f021-438d-9f84-6aefd0ade54d" />

1. Cp -r Unix/TP1 Unix/TP2 Python : Je copie TP1 dans le repertoire Unix/TP1 et idem pour TP2 pour aller vers le dossier Python.

Sous Etape 4 : Créer deux répertoire séance_1 et séance_2 dans le dossier TP1 de Unix : 

<img width="753" height="181" alt="image" src="https://github.com/user-attachments/assets/0e494d10-36e6-47c1-be00-5fab9b0f419d" />

1. mkdir seance_1 seance_2 : Créer les dossier seance_1 et seance_2
2. ls : Permet de confirmer que les dossier ont bien été créer.
3. cd seance_1 : Confirme que seance-1 est bien la puisque je peux naviguer dans le dossier.

Sous Etape 5 : Créer deux fichiers exo1 et exo2 dans le répertoire séance 1 : 

<img width="836" height="191" alt="image" src="https://github.com/user-attachments/assets/0700183c-9285-48b0-a061-fc76c204dce4" />

1. cd seance_1 : JE rentre dans le dossier seance_1
2. touch exo1.txt exo2.txt : Je créer les deux fichier exo1 et exo2.txt
3. ls : Permet de confirmer que exo1.txt et exo2.txt ont bien étaient créer.

Sous Etape 6 : Copier les deux fichiers exo1.txt et exo2.txt dans le répertoire TP2 de Python.

<img width="1034" height="247" alt="image" src="https://github.com/user-attachments/assets/0707fb7b-02fd-405c-b601-ec9e7e916914" />

1. cp -r Unix/TP1/seance_1/exo1.txt Unix/TP1/seance_1/exo2.txt Python/TP2 : Je copie les deux fichiers qui sont au bout du chemin, puis je les intègre dans Dans Python/TP2.
2. cd  Python/TP2 : Je me déplace dans le dossier TP2
3. ls : Je peux confirmer qu'ils ont bien été copié dans le fichiers demandé.

Sous Etape 7 : Depuis Unix/TP2 me déplacer dans Python/TP1 en utilisant le chemin relatif, puis retourner sur Unix/TP2.

<img width="702" height="166" alt="image" src="https://github.com/user-attachments/assets/a7e67553-5abd-4126-a9f7-aa0d3a2a5dc4" />

Je suis passer de Unix/TP2 a Python/TP1 en utilisant le chemin relatif

<img width="831" height="80" alt="image" src="https://github.com/user-attachments/assets/6fbc9843-cef9-4ffc-98b7-70102f94fbc3" />

Et voila comment re-changer en utilisant le chemin absolu

 Sous Etape 8 : Supprimer le répertoire TP1 de Python 

 <img width="633" height="133" alt="image" src="https://github.com/user-attachments/assets/6c1eabc7-e924-4d97-a984-6c32f8d61710" />

 1. rmdir TP1 : Efface le dossier TP1 dans le chemin actuel où je me trouve.
 2. ls : Confirme que TP1 a bien été supprimé.

Sous Etape 9 : Supprimer le répertoire TP2 de Python : 

<img width="597" height="105" alt="image" src="https://github.com/user-attachments/assets/fada58d8-a5f8-4e8f-8ea2-f1bb5885ee1a" />

1. La suppression est en échec, normal : Le dossier n'est pas vide !

<img width="836" height="175" alt="image" src="https://github.com/user-attachments/assets/0f5fe364-511d-46dd-96b5-2b9568ebe406" />

1. rm exo1.txt exo2.txt : Je supprime les deux exos
2. cd .. : je recule d'un dossier sur le chemin
3. rmdir TP2 : Supprime TP2
4. ls : confirme que plus rien n'est dans le dossier.
5. Aussi possible et plus rapide avec une seule commande 'rm -r TP2'

Sous Etape 10 : Déplacer le fichier exo1 dans le répertoire TP1 et supprimer les répertoires séance 1 et séance 2.

<img width="838" height="439" alt="image" src="https://github.com/user-attachments/assets/d69fcb55-0c20-454e-b31f-4c8ef5788da6" />

1. mv seance_1/exo.txt TP1 : Déplace seance_1/exo1.txt dans le dossier TP1.
2. ls : Conforme ce mouvement
3. mv TP1 exo1.txt : Déplace exo1.txt dans TP1
4. rm seance_1 seance_2 : Supprime seance_1 et seance_2
5. Observation : Je ne peux pas les supprimer.
6. rm -r seance_1 seance_2 : Supprime vraiment seance_1 et seance_2 sans message d'erreur avec le 'r' de récursif
7. ls : Confirme que c'est bien surppimé.

Etape 2 : Protection des fichiers 

