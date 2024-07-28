## Docker-Static-WebApp

Ce projet a pour but de conteneuriser à l'aide de Docker le site web d'une entreprise X. Pour se faire, nous avons procédé comme suit: 



#### Étape 1 : rédaction du Dockerfile
 
Dans ce fichier nous clonons le code source du site disponible à l'adresse:

 ```(https://github.com/diranetafen/static-website-example.git)```

#### Étape 2 : Création de l'image
```docker build -t static-webapp:v1 .```

#### Étape 3 : Test de l'image

```docker run --name static-webapp -d -p 80:80 static-webapp:v1```

#### Étape 4 : Push de l'image sur le Docker Hub

```docker push linanzouechim/static-webapp:v1``` 