# PLEX HOMESERVER

## _Descripcion_
Plex Home Server es un proyecto de código abierto que permite a los usuarios tener una experiencia completa para administrar un servicio multimedia y poder arrancarlo desde docker. 
>Hay que tener en cuenta que este servicio está orientado a ser usado en servidores propios.
Todo este sistema se basa en una gestión a través de applicaciones independientes encapsuladas en contenedores de Docker por lo que es necesario tener este sistema instalado en el ordenador/servidor donde se vaya a correr. Para eso se puede realizar mediante [Docker Desktop](https://www.docker.com/products/docker-desktop/) o mediante línea de comandos.

Este proyecto contiene lo siguiente:

- Plex: Servicio multimedia de Streaming gratuito para poder consumir series, peliculas y otras archivos.
- Radarr: Servicio que permite la busqueda de películas en formato torrent.
- Sonarr: Servicio que permite la busqueda de series en formato torrent.
- Transmission: Servicio que permite descargar de manera automática los archivos torrent.
## _Uso_
Antes de levantar el proyecto se deberá generar un archivo ```.env``` siguiendo el ejemplo de [.env.example](./.env.example), dentro del mismo archivo hay unas indicaciones a seguir.

Luego es tan sencillo como levantar el proyecto en Docker usando el comando ```docker compose up -d```. 
Para acceder a los diferentes servicios te dejo los links a continuación:

- [Plex](http://localhost:32400/web)
- [Radarr](http://localhost:7878)
- [Sonarr](http://localhost:8989)
- [Transmission](http://localhost:9091/)
  - user: admin
  - password: 123456