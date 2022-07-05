# Keycloak

## Initialize Spring Boot project

```sh
curl -s -O https://start.spring.io/starter.zip \
         -d type=maven-project \
         -d language=java \
         -d platformVersion=2.7.1 \
         -d packaging=jar \
         -d jvmVersion=11 \
         -d groupId=dev.mikoto2000.study.springboot.keycloak \
         -d artifactId=gettingstarted \
         -d name=gettingstarted \
         -d description=Demo%20project%20for%20Spring%20Boot%20with%20Keycloak \
         -d packageName=dev.mikoto2000.study.springboot.keycloak.gettingstarted \
         -d dependencies=thymeleaf,web

unzip starter.zip -d project/

rm starter.zip
```

## Start Development environment

```sh
docker compose up -d
```


## Build project

### Interactive

```sh
docker compose exec java bash
```

### Run Spring Boot project

```sh
docker compose exec java ./mvnw spring-boot:run
```

### Build Spring Boot project

```sh
docker compose exec java ./mvnw spring-boot:repackage
```

## Stop Development environment

```sh
docker compose down
```

