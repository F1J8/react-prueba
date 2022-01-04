# Prueba de React *(Free Games)*
## Acerca de la prueba
Desarrolle una aplicación en react que se conecte con API para listar y ver detalles de juegos gratis

### Páginas
* Página con lista de juegos
* Página detallada de cada juego

### Página de lista
* Listar los juegos con limite de 10
* Mostrar imagen de thumbnail para cada juego
* Filtrar según plataforma o categoría
 ```sh
Endpoint: GET https://www.freetogame.com/api/games
```
* Ejemplo de un item:
``` json
{
    "id": 515,
    "title": "Halo Infinite",
    "thumbnail": "https://www.freetogame.com/g/515/thumbnail.jpg",
    "short_description": "For the first time ever, a free-to-play Halo experience is available in the form of Halo Infinite’s multiplayer.",
    "game_url": "https://www.freetogame.com/open/halo-infinite",
    "genre": "Shooter",
    "platform": "PC (Windows)",
    "publisher": "Xbox Game Studios",
    "developer": "343 Industries",
    "release_date": "2021-11-15",
    "freetogame_profile_url": "https://www.freetogame.com/halo-infinite"
  }
```
### Página con detalles de un juego
* Mostrar todos los detalles del juego
* Mostrar screenshots del juego
* Mostrar los requisitos mínimos del juego 
 ```sh
Endpoint: GET https://www.freetogame.com/api/game?id=515
Utilizar el game id
```
* Ejemplo de un item:
``` json
{
  "id": 515,
  "title": "Halo Infinite",
  "thumbnail": "https://www.freetogame.com/g/515/thumbnail.jpg",
  "status": "Live",
  "short_description": "For the first time ever, a free-to-play Halo experience is available in the form of Halo Infinite’s multiplayer.",
  "description": "For the first time ever, a free-to-play Halo experience is available in the form of Halo Infinite’s multiplayer. 343 Industries and Xbox Game Studios made the multiplayer version of the game available separately from the full story campaign, which is available to purchase for $60 to allow everyone to get in on the action. With the multiplayer, players can take part in two different modes: Arena and Big Team Battle. The first returns to Halo’s multiplayer roots with on-map equipment and 4-player squads. Big Team Battle allows players to mix and match weapons, vehicles and equipment to create a unique combat experience.\r\n\r\nThe game also offers players the ability to customize their Spartan with cosmetic items. Of course, those with the campaign will have access to extra options. Even more can be found in the game’s battle pass which also introduces new modes and maps, as well as community-focused content.\r\n",
  "game_url": "https://www.freetogame.com/open/halo-infinite",
  "genre": "Shooter",
  "platform": "Windows",
  "publisher": "Xbox Game Studios",
  "developer": "343 Industries",
  "release_date": "2021-11-15",
  "freetogame_profile_url": "https://www.freetogame.com/halo-infinite",
  "minimum_system_requirements": {
    "os": "Windows 10 RS5 x64",
    "processor": "AMD Ryzen 5 1600 or Intel i5-4440",
    "memory": "8 GB RAM",
    "graphics": "AMD RX 570 or Nvidia GTX 1050 Ti",
    "storage": "50 GB available space"
  },
  "screenshots": [
    {
      "id": 1253,
      "image": "https://www.freetogame.com/g/515/Halo-Infinite-1.jpg"
    },
    {
      "id": 1254,
      "image": "https://www.freetogame.com/g/515/Halo-Infinite-2.jpg"
    },
    {
      "id": 1255,
      "image": "https://www.freetogame.com/g/515/Halo-Infinite-3.jpg"
    }
  ]
}
```
#### Otros Endpoints
``` ssh
Games by platform
GET https://www.freetogame.com/api/games?platform=pc
Insert platform, eg: pc, browser or all
```
``` ssh
Games by category or tag
GET https://www.freetogame.com/api/games?category=shooter
Insert game category or tag, eg: mmorpg, shooter, pvp, mmofps
```
#### Para más detalles del API:
* [https://www.freetogame.com/api-doc](https://www.freetogame.com/api-doc)
#### Sitio web de referencia:
* [https://www.freetogame.com/](https://www.freetogame.com/)
* [https://www.freetogame.com/halo-infinite](https://www.freetogame.com/halo-infinite)
## Requisitos

Deberás tener instalado las siguientes versiones de librerías para ello.

* Node JS / latest
* NPM / latest
* Git / latest

#### Evitar utilizar frameworks o librerías de estilo *(Boostrap/Foundation)* utilizar css/scss
#### Al finalizar subir el contenido a un repositorio público y enviar el enlace. 
* *(Opcional)* Publicar en Cloudflare Pages / Github Pages / Heroku / etc
* *(Opcional)* Integrar Redux
* *(Opcional)* Integrar Sentry
