# Serviços

## Tarefa 1

![Componentes de Negócio](https://github.com/jhowmerisse/INF331-labs/blob/master/lab04%20-%20servicos/images/Componentes%20de%20neg%C3%B3cio.png)

## Tarefa 2

![Componentes Técnicos - ( Controller e View)](https://github.com/jhowmerisse/INF331-labs/blob/master/lab04%20-%20servicos/images/Componentes%20t%C3%A9cnicos%20-%20Controller%20View.png)

## Tarefa 3

![Componentes Técnicos - ( Model e Controller)](https://github.com/jhowmerisse/INF331-labs/blob/master/lab04%20-%20servicos/images/Componentes%20t%C3%A9cnicos%20-%20Model%20Controller.png)

## Tarefa 4

### Serviço 1:

#### Título do serviço: 
The Open Targets Platform REST API

#### URI do serviço:
http://api.opentargets.io/v3/platform/public/search?q=covid&size=10&from=0&filter=disiase

#### Descrição:
A API Open Targets Platform ('Interface de Programação de Aplicativo') permite a recuperação programática de nossos dados por meio de um conjunto de serviços REST .
Este método permite que você procure genes ou doenças de interesse usando uma pesquisa de texto livre, replicando a funcionalidade da caixa de pesquisa em nossa página inicial. Deve ser usado para identificar a melhor correspondência para uma doença ou alvo de interesse, em vez de reunir um conjunto específico de evidências.

#### General:
~~~~http
Request URL: http://api.opentargets.io/v3/platform/public/search?q=covid&size=10&from=0&filter=disiase
Request Method: GET
Status Code: 200 OK
Remote Address: 35.227.220.99:80
Referrer Policy: no-referrer-when-downgrade
~~~~

### Request Headers: 
~~~~http
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36
~~~~

#### Query String Parameters:
~~~~http
q: covid
size: 10
from: 0
filter: disiase
~~~~

#### Response Headers:
~~~~http
Access-Control-Allow-Headers: Content-Type,Auth-Token
Access-Control-Allow-Methods: GET,PUT,POST,DELETE,OPTIONS
Access-Control-Allow-Origin: *
Cache-Control: public, no-transform, max-age=2592000
Content-Encoding: gzip
Content-Type: application/json
Date: Fri, 28 Aug 2020 17:31:26 GMT
Server: nginx
Vary: Accept-Encoding
Via: 1.1 google
~~~~
#### Response:
~~~~json
{
  "data_version": "20.06",
  "from": 0,
  "suggest": [
    "colic",
    "corin",
    "cord",
    "cold",
    "coli"
  ],
  "facets": [],
  "total": 0,
  "data": [],
  "took": 0,
  "size": 0
}
~~~~

### Serviço 2:

#### Título do serviço: 
API Icons8

#### URI do serviço:
https://api.icons8.com/api/iconsets/v3/categories?platform=win10&language=pt-BR

#### Descrição:
Icons8 API Icons8 API nos permite pesquisar e obter nossos ícones. Você pode usar nossos ícones para estender a funcionalidade de seus aplicativos da web e móveis, modelos de sites e até tatuagens.
A operação não retornará as categorias que possuem menos de 10 ícones. 

#### General:
~~~~http
Request URL: https://api.icons8.com/api/iconsets/v3/categories?platform=win10&language=pt-BR
Request Method: GET
Status Code: 200 OK
Remote Address: 148.72.173.7:443
Referrer Policy: no-referrer-when-downgrade
~~~~

### Request Headers: 
~~~~http
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Accept-Encoding: gzip, deflate, br
Accept-Language: en-US,en;q=0.9,pt;q=0.8
Connection: keep-alive
Host: api.icons8.com
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: none
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36
~~~~

#### Query String Parameters:
~~~~http
platform: win10
language: pt-BR
~~~~

#### Response Headers:
~~~~http
Access-Control-Allow-Credentials: true
Access-Control-Allow-Headers: DNT,X-CustomHeader,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type,Client-App
Access-Control-Allow-Methods: HEADER,OPTIONS,GET,PUT
Access-Control-Allow-Origin: https://icons8.com.br
Access-Control-Max-Age: 86400
Cache-control: must-revalidate
Connection: keep-alive
Content-Encoding: gzip
Content-Type: application/json
Date: Fri, 28 Aug 2020 17:49:06 GMT
Expires: Sat, 29 Aug 2020 17:49:06 GMT
Server: nginx
Transfer-Encoding: chunked
Vary: Accept-Encoding
~~~~
#### Response:
~~~~json
{
  "success": true,
  "result": {
    "categories": [
      {
        "name": "Alfabeto",
        "api_code": "alphabet",
        "free": 0
      },
      {
        "name": "Animais",
        "api_code": "animals",
        "free": 0
      },
      {
        "name": "Arquivos",
        "api_code": "files",
        "free": 0
      },
      {
        "name": "Astrologia",
        "api_code": "astrology",
        "free": 0
      },
      {
        "name": "Bebidas",
        "api_code": "drinks",
        "free": 0
      },
      {
        "name": "Bebê",
        "api_code": "baby",
        "free": 0
      },
      {
        "name": "Beleza",
        "api_code": "beauty",
        "free": 0
      },
      {
        "name": "Casas",
        "api_code": "household",
        "free": 0
      },
      {
        "name": "Characters",
        "api_code": "characters",
        "free": 1
      },
      {
        "name": "Cidade",
        "api_code": "city",
        "free": 0
      },
      {
        "name": "Cinema",
        "api_code": "cinema",
        "free": 0
      },
      {
        "name": "Ciências",
        "api_code": "science",
        "free": 0
      },
      {
        "name": "Clima",
        "api_code": "weather",
        "free": 0
      },
      {
        "name": "Comida",
        "api_code": "food",
        "free": 0
      },
      {
        "name": "Compras",
        "api_code": "shopping",
        "free": 0
      },
      {
        "name": "Comércio eletrônico",
        "api_code": "ecommerce",
        "free": 0
      },
      {
        "name": "Controles de mídia",
        "api_code": "media_controls",
        "free": 0
      },
      {
        "name": "Crime",
        "api_code": "crime",
        "free": 0
      },
      {
        "name": "Culture",
        "api_code": "cultures",
        "free": 0
      },
      {
        "name": "Dados",
        "api_code": "data",
        "free": 0
      },
      {
        "name": "Data e hora",
        "api_code": "time_and_date",
        "free": 0
      },
      {
        "name": "Edição",
        "api_code": "editing",
        "free": 0
      },
      {
        "name": "Esportes",
        "api_code": "sports",
        "free": 0
      },
      {
        "name": "Faça você mesmo",
        "api_code": "diy",
        "free": 0
      },
      {
        "name": "Feriados",
        "api_code": "holidays",
        "free": 0
      },
      {
        "name": "Finanças",
        "api_code": "finance",
        "free": 0
      },
      {
        "name": "Flags",
        "api_code": "flags",
        "free": 0
      },
      {
        "name": "Foto e Vídeo",
        "api_code": "photo_video",
        "free": 0
      },
      {
        "name": "Hardware",
        "api_code": "computer_hardware",
        "free": 0
      },
      {
        "name": "Impressão",
        "api_code": "printing",
        "free": 0
      },
      {
        "name": "Indústria",
        "api_code": "industry",
        "free": 0
      },
      {
        "name": "Interface de usuário",
        "api_code": "user_interface",
        "free": 0
      },
      {
        "name": "Jogos",
        "api_code": "gaming",
        "free": 0
      },
      {
        "name": "Logotipos",
        "api_code": "logos",
        "free": 1
      },
      {
        "name": "Mapas",
        "api_code": "maps",
        "free": 0
      },
      {
        "name": "Mensagens",
        "api_code": "messaging",
        "free": 0
      },
      {
        "name": "Militar",
        "api_code": "military",
        "free": 0
      },
      {
        "name": "Mobile",
        "api_code": "mobile",
        "free": 0
      },
      {
        "name": "Mãos",
        "api_code": "hands",
        "free": 0
      },
      {
        "name": "Músicas",
        "api_code": "music",
        "free": 0
      },
      {
        "name": "Negócios",
        "api_code": "business",
        "free": 0
      },
      {
        "name": "Pastas",
        "api_code": "folders",
        "free": 0
      },
      {
        "name": "Perfil",
        "api_code": "profile",
        "free": 0
      },
      {
        "name": "Pessoas",
        "api_code": "users",
        "free": 0
      },
      {
        "name": "Plantas",
        "api_code": "plants",
        "free": 0
      },
      {
        "name": "Popular Icons",
        "api_code": "free_icons",
        "free": 1
      },
      {
        "name": "Programação",
        "api_code": "programming",
        "free": 0
      },
      {
        "name": "Rede",
        "api_code": "network",
        "free": 0
      },
      {
        "name": "Roupas",
        "api_code": "clothing",
        "free": 0
      },
      {
        "name": "Saúde",
        "api_code": "healthcare",
        "free": 0
      },
      {
        "name": "Segurança",
        "api_code": "security",
        "free": 0
      },
      {
        "name": "Setas",
        "api_code": "arrows",
        "free": 0
      },
      {
        "name": "Sistemas operacionais",
        "api_code": "operating_systems",
        "free": 0
      },
      {
        "name": "Social Media",
        "api_code": "social_networks",
        "free": 0
      },
      {
        "name": "Transportes",
        "api_code": "transport",
        "free": 0
      },
      {
        "name": "Viagem",
        "api_code": "travel",
        "free": 0
      }
    ]
  }
}
~~~~
