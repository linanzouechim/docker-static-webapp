## Docker-Static-WebApp

Ce projet a pour but de conteneuriser à l'aide de Docker le site web d'une entreprise X. Pour se faire, nous avons procédé comme suit: 

Ce projet consiste à créer une image Docker et la publier sur Docker Hub en suivant les étapes suivantes : 

#### Étape 1 : rédaction du Dockerfile

```vi Dockerfile``` 
Dans ce fichier nous clonons le code source du site disponible à l'adresse: ```(https://github.com/diranetafen/static-website-example.git)```

#### Étape 2 : Instructions Docker

Renseigner les [instructions](https://github.com/MozkaGit/devops-bootcamp-docker/blob/b497f0315498d08df5b992f5708a982b19cd7253/TP2/Dockerfile) Docker souhaités puis enregistrer le fichier.


#### Étape 3 : Création de l'image

```docker build -t webapp:v1 .```

#### Étape 5 : Test de l'image

Avec la commande suivante :

```docker run --name webapp -d -p 80:80 webapp:v1```

#### Étape 6 : Déploiement de l'image Docker Hub

```docker push mozkadocker/webapp:v1```

----

### Divers

1) Il est possible d'automatiser le déploiement des images sur Docker Hub grâce à GitHub mais malheureusement il ne sera pas possible de le faire maintenant car c'est devenu une fonctionnalité payante.

2) Voici mon dépôt Docker pour ce TP => https://hub.docker.com/r/mozkadocker/webapp