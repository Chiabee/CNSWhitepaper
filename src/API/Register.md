# Register

## Price

Get the price for domain registering.

**GET** https://cns.api.pawket.app/api/price

**Request:**

```text
?name=123458.xch&year=1&renew=false
```

| Key   | Required? | Description                                        |
| ----- | --------- | -------------------------------------------------- |
| name  | Yes       | the name to register, typically suffix with `.xch` |
| year  | Yes       | how many year to register or renew, max 99         |
| renew | No        | whether to get price for register or renew         |

**Response:**

```json
{
  "name": "123458.xch",
  "price": 400000000000,
  "annualFee": 250000000000,
  "registrationFee": 150000000000,
  "royaltyPercentage": 500,
  "success": true
}
```

| Key               | Type     | Description                                    |
| ----------------- | -------- | ---------------------------------------------- |
| name              | String   | the name to register or renew                  |
| price             | Number   | the total price for register or renew, in mojo |
| annualFee         | Number   | the annual fee for this name, in mojo          |
| registrationFee   | Number   | the registration fee for this name, in mojo    |
| royaltyPercentage | Number   | the royalty percentage in 1/10000, e.g. 500=5% |
| success           | Boolean  | whether success to get price information       |
| code              | String   | if failed, this is the error code              |
| reason            | String   | if failed, this is the reason                  |
| arguments         | String[] | if failed, this is the arguments for reason    |

## Register

Get the offer for registering or renewing.

**POST** https://cns.api.pawket.app/api/register

**Request:**

```json
{
  "name": "123458.xch",
  "royaltyAddress": "",
  "address": "",
  "publicKey": "",
  "did": "",
  "text": "",
  "renew": false,
  "year": 1
}
```

| Key            | Required? | Description                                                          |
| -------------- | --------- | -------------------------------------------------------------------- |
| name           | Yes       | the name to register, typically suffix with `.xch`                   |
| year           | Yes       | how many year to register or renew, max 99                           |
| royaltyAddress | No        | the default royalty address of this CNS NFT, format like xch1...     |
| address        | No        | the default binding address, format like xch1                        |
| publicKey      | No        | the default binding publick key, format usually like 0x...           |
| did            | No        | the default binding DID, format like did:chia:...                    |
| text           | No        | the default binding text, can be arbitrary text except double quotes |
| renew          | No        | whether to get price for register or renew                           |

**Response:**

```json
{
  "name": "123458.xch",
  "offer": "offer1qqr83....",
  "image": "/9j/4AAQSkZJRg....",
  "success": true
}
```

| Key       | Type     | Description                                 |
| --------- | -------- | ------------------------------------------- |
| name      | String   | the name to register or renew               |
| image     | String   | the NFT image in base64                     |
| offer     | String   | the offer string                            |
| success   | Boolean  | whether success to get register offer       |
| code      | String   | if failed, this is the error code           |
| reason    | String   | if failed, this is the reason               |
| arguments | String[] | if failed, this is the arguments for reason |
