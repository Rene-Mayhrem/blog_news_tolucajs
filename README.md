# Feed de noticias | tolucajs

Bienvenidos a este proyecto open-source donde el objetivo es contruir un feed de noticias functional construido usando una API desarrollada enn NestJS y siendo consumida por un servicio de frontend con el framework de VueJs.

## Prerequisitios

- docker

Este proyecto ha sido creado con contenedores para su simplificación, así que en caso de que no cuentes con docker instalado, aquí agrego la liga del manual de instalación.

[Docker para Windows](https://docs.docker.com/desktop/install/windows-install/)

[Docker para Mac](https://docs.docker.com/desktop/install/mac-install/)

[Docker para Linux](https://docs.docker.com/desktop/install/linux-install/)

## Consideraciones

Las especificaciones de los servicios, así como los puertos utilizados, lo puedes encontrar en los siguientes archivos

- [docker-compose.yml](docker-compose.yml)
- [Dockerfile para backend](./backend/Dockerfile)
- [Dockerfile para frontend](./frontend/Dockerfile)

## Getting started

Para iniciar la aplicación, es necesario contar con el comando **docker compose** o su equivalente **docker-compose** y usar la siguiente instrucción en una terminal

```
docker compose up
```

El comando *docker compose up* construirá dos servicios, uno de frontend y otro de backend.

Para la parte del backend el servicio será creado en el puerto 3000 y será un servicio de NestJS, así que asegúrate de tener disponible ese puerto o en su caso, modificar el archivo _docker-compose.yml_ para seleccionar un puerto disponible, para verificar que este funcionando este servicio, puedes consultar http://localhost:3000

Para el servicio de frontend, se ha utilizado un contenedor que correrá Vuejs, de igual manera, debes de considerar el puerto en uso 8080, porque este es el especificado, para comprobar el funcionamiento del servicio, consulta la siguiente liga http://localhost:8080
