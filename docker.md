# Image

Un fichier qui contient le code source, les librairies, les dépendances et les outils, tout ce qui permet de run l'application. On ne peut pas executer directement une image, c'est un modèle qui permet de créer un container. une image est immuable on ne peut pas la modifier, lorsque l'on run un container on créer une copie de l'image modifiable cette fois-ci.

# Container

Un conteneur docker est un environnement d'execution virtualizé dans lequel on peut isoler les application. c'est une unité compacte et portable dans laquelle on peut run une application facilement et rapidement. il permet de standardiser l'environnement et garantit le fonctionnement de l'application même en le partageant à d'autre personnes.

# Commandes

## build

docker build permet de créer des images docker à partir d'un Dockerfile et d'un contexte (qui représente l'ensemble des fichiers situés dans le path ou l'url).

## run

docker run permet de créer un container sur l'image spécifiée puis de démarrer l'application.

## exec

docker exec permet d'exécuter une nouvelle commande dans un container en cours.