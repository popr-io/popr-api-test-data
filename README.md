# popr-api-test-data
Test data for the POPr api

A website for this repository can be found at [https://popr-io.github.io/popr-api-test-data/]

The hashes in a POPr receipt use the sha256 hashing algorithm. Hashes can be tested with the following tools:
- openssl: echo -n "string" | openssl dgst -sha256
- sha256sum (linux): echo -n "string" | sha256sum
- shasum (OSX): echo -n "string" | shasum -a 256 -t -
- /sha256.html on this site

The receipt serializing and hashing can be tested on the /hash.html page on this site.

Example:
```
{
  "time": 1560100862,
  "retailerId": "popr-test-store",
  "shopId": "1",
  "terminalId": "POS1",
  "employeeId": "ams25522",
  "invoiceId": "1212",
  "totalValue": 10865,
  "totalVAT": 1886,
  "vatLines": [
    {
      "vat": 2100,
      "vatAmount": 1886
    }
  ],
  "lines": [
    {
      "productId": "4022",
      "description": "Keychain CITIES 3Cha",
      "amount": 495,
      "vat": 2100,
      "vatAmount": 86,
      "number": 1
    },
    {
      "productId": "4688",
      "description": "Opener Window STAR G",
      "amount": 995,
      "vat": 2100,
      "vatAmount": 173,
      "number": 1
    },
    {
      "productId": "4690",
      "description": "Iphone 10 Green",
      "amount": 1295,
      "vat": 2100,
      "vatAmount": 225,
      "number": 1
    },
    {
      "productId": "4339",
      "description": "Bag Reusable Shopper",
      "amount": 590,
      "vat": 2100,
      "vatAmount": 102,
      "number": 1
    },
    {
      "productId": "3748",
      "description": "Umbrella Green Big",
      "amount": 2495,
      "vat": 2100,
      "vatAmount": 433,
      "number": 1
    },
    {
      "productId": "3552",
      "description": "Speaker Mini NJOY Bl",
      "amount": 4995,
      "vat": 2100,
      "vatAmount": 867,
      "number": 1
    }
  ]
}

```

string: 1560100862/popr-test-store/1/POS1/1212/10865/1886////
hash: ebc0b790a210d014fd16f9facf2d10cd17dc74515a9392bb65d51fefe6f441f4
hashSignature: 4d217216d07d1e7141cba8ee72097462f684cc06f1577f664f9d1628ae20dba6
