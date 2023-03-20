# Bins-API

Una API para obtener detalles de BIN o tarjetas de Crédito o Débito.

---

## API

Enviar solicitud de obtención a `http://yourhost:port/api/{bin}`

## Ejemplo

Obtener API en : `https://bin.jcystem.com/API/549184`

Respuesta : 

```json
{
    "result": true,
    "message": "Search Successful",
    "data": {
        "bin": "549184",
        "vendor": "MASTERCARD",
        "type": "DEBIT",
        "level": "PLATINUM",
        "bank": "BANK NIZWA SAOG",
        "country": "OMAN",
        "countryInfo": {
            "name": "OMAN",
            "emoji": "🇴🇲",
            "unicode": "U+1F1F4 U+1F1F2",
            "code": "OM",
            "dialCode": "+968"
        }
    }
}
```

#### Errors :

```json
// No Results Found
{"result":false,"message":"No Results Found"}

// Invalid Bin
{"result":false,"message":"Request a Valid BIN"}
```

---

## Instalación Local

```bash
$ git clone https://github.com/srnovus/bin-api/
$ cd bins-su-api
$ npm install 
$ npm start
```

Su aplicación ahora debería estar ejecutándose en [localhost:3000](http://localhost:3000/).

---

## Deploy
| Heroku | Vercel |
| :---: | :---: |
| [![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy) | [![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/srnovus/bin-api) |

`Nota: el raspado no es un uso justo de Vercel`

