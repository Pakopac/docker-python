# Image

Un fichier qui contient le code source, les librairies, les dépendances et les outils, tout ce qui permet de run l'application. On ne peut pas executer directement une image, c'est un modèle qui permet de créer un container. une image est immuable on ne peut pas la modifier, lorsque l'on run un container on créer une copie de l'image modifiable cette fois-ci.

# Container

Un conteneur docker est un environnement d'execution virtualizé dans lequel on peut isoler les application. c'est une unité compacte et portable dans laquelle on peut run une application facilement et rapidement. il permet de standardiser l'environnement et garantit le fonctionnement de l'application même en le partageant à d'autre personnes.

# Commandes

## Build

Docker build permet de créer des images docker à partir d'un Dockerfile et d'un contexte (qui représente l'ensemble des fichiers situés dans le path ou l'url).

## Run

Docker run permet de créer un container sur l'image spécifiée puis de démarrer l'application.

## Exec

Docker exec permet d'exécuter une nouvelle commande dans un container en cours.

## Start/stop

Docker start/stop permet de démarrer/stopper un conteneur

```
Docker build -t python-app .
```

Build un conteneur spécifique

```
Docker run -d -p 5000:5000 python-app
```

Run le conteneur en deamon sur le port 5000 

# Déploiement Heroku

```
heroku container:login
```
Connection à heroku

```
heroku container:push web
heroku container:release web
```
Envoie du code à heroku