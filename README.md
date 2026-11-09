# mon-service

Mini application Spring Boot (Java 25, Gradle) avec un endpoint `/hello`.

## Lancer en local

```
cd mon-service
./gradlew bootRun
```

Puis ouvrir http://localhost:8080/hello

## Docker

Construire l'image :

```
cd mon-service
docker build -t wiemmben/mon-service:1.0 .
```

Lancer le conteneur :

```
docker run -p 8080:8080 wiemmben/mon-service:1.0
```

Publier sur Docker Hub :

```
docker login
docker push wiemmben/mon-service:1.0
```

Image : https://hub.docker.com/r/wiemmben/mon-service