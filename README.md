# firebase-tools
Image docker para Firebase Tools

## Tags soportado en Dockerfile

- `6`, `latest` [6/Dockerfile](https://github.com/mvochoa/firebase-tools/blob/master/6/Dockerfile)

## Ejemplo de `docker-compose.yml`

```
version: '3.3'
services:
    server:
        image: mvochoa/firebase-tools
        volumes:
            - ./:/var/app
        ports:
            - 5000:5000
        command: ["firebase", "serve", "-o", "0.0.0.0"]
```
