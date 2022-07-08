## API

Send Get Request to `http://yourhost:port/api/{bin}`


Response : 

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

## Deploy
| Heroku |
| :---: | :---: |
| [![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy) 

