# TP 1 – Découverte de l’environnement Linux

## Présentation

Ce laboratoire a pour objectif de prendre en main l'administration d'un système Linux (Debian/Ubuntu) exclusivement en ligne de commande. Il couvre les fondamentaux indispensables à la gestion d'un serveur : identification du système, navigation dans l'arborescence standard, manipulation de fichiers, gestion des permissions de sécurité (chmod et privilèges sudo), supervision des ressources et déploiement de paquets via le gestionnaire apt

## Objectifs

*  Identifier les caractéristiques du système et de l'utilisateur courant (uname, os-release, whoami).
*  Maîtriser la navigation dans l'arborescence des répertoires et l'usage de l'aide en ligne (man, --help)
*  Manipuler fichiers et flux de redirection (touch, cp, mv, >, >>)
*  Analyser et modifier les droits d'accès aux fichiers en notations symbolique et octale (chmod 600).
*  Superviser l'état du système (processus, mémoire, disque et réseau via ip a, df, free).
*  Gérer l'installation de logiciels avec le gestionnaire de paquets apt.

## Déroulement du laboratoire


### Étape 1

Identifier le systéme : 

Executer différentes commandes sur l'invit de commande, observer les resultat et ce qu'il indique.

Whoami : Cette commande sert a savoir qui est l'utilisateur qui utilise cette commande. Ici en l'occurence, thibault (moi).

<img width="469" height="188" alt="image" src="https://github.com/user-attachments/assets/392fcbd6-7174-41f8-9663-0712f4effcc2" />


Hostname : Cette commande sert a savoir le nom de l'appareil.

<img width="761" height="153" alt="image" src="https://github.com/user-attachments/assets/b2f29ad9-8073-4ca8-a97c-8cdc95b43a26" />


cat /etc/os-release : Utile pour connaitre la version du système d'exploitation. Je sais par exemple que je suis sur la version 26.04.1 LTS de Ubuntu (PRETTY_NAME)

<img width="1047" height="307" alt="image" src="https://github.com/user-attachments/assets/a810711a-a109-4fa9-a5e0-a3937302e60f" />


uname -r : Donne la version Linux actuel : 

<img width="1047" height="307" alt="image" src="https://github.com/user-attachments/assets/42cad119-ed4a-4545-93cc-86a80bfc005e" />

date : Utile pour connaitre la date.

<img width="604" height="52" alt="image" src="https://github.com/user-attachments/assets/e77a6a37-d3ce-4730-8600-f4ae091ee6fc" />


### Étape 2

Naviguer dans l’arborescence : 

pwd : Affiche le répertoire courant.

<img width="624" height="56" alt="image" src="https://github.com/user-attachments/assets/2ad2ab09-4c2e-446a-af13-205141296531" />


ls : Liste le contenu d'un dossier

<img width="1349" height="51" alt="image" src="https://github.com/user-attachments/assets/57eb8fb4-ca75-445a-ba32-164390c1e03c" />


ls -l : Liste le contenu d'un dossier détaillé.

<img width="789" height="330" alt="image" src="https://github.com/user-attachments/assets/2d0c02bd-c0d3-47be-9884-97f85b710e68" />


ls -a : Liste le contenue d'un dossier, mais uniquement les fichiers cachés.

<img width="1402" height="70" alt="image" src="https://github.com/user-attachments/assets/2299b9b1-8e84-4517-9bb4-7d3227c902a9" />


cd / + ls : cd / s'utilise pour changer de répertoire, et ls Liste le contenu du répertoire qui viens de changer. 


<img width="1655" height="71" alt="image" src="https://github.com/user-attachments/assets/22425978-6c1c-4fa0-a159-4fafc8a29a34" />

Je remarque également que cd.. recul d'un dossier, et cd ~ recul jusqu'au dossier de base.



### REPRENDRE AU NIVEAU DE LA QUESTION 3 DU DOC. ###

**Observation :** [Explication du résultat obtenu.]

### Étape 2.1

[Sous-étape ou test de vérification complémentaire.]

<img width="600" alt="Capture étape 2.1" src="[LIEN_DE_TON_IMAGE_GITHUB]" />

**Observation :** [Analyse du comportement de l'équipement ou du paquet.]

## Commandes utilisées

<img width="800" alt="Tableau des commandes" src="[LIEN_DE_TON_IMAGE_GITHUB]" />

*(Optionnel si tu n'as pas de capture : tu peux aussi lister tes commandes dans un bloc de code texte).*

## Ce que j'ai appris

[Paragraphe expliquant les notions théoriques et pratiques que tu as comprises grâce à ce lab.]

## Difficultés rencontrées

[Le problème ou la confusion rencontrée lors de la manipulation, et l'explication technique de comment tu l'as résolu ou compris.]

## Conclusion

[Bilan global du laboratoire et validation des objectifs fixés.]

## Fin de ce laboratoire
