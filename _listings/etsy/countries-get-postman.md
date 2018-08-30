{
  "info": {
    "name": "Etsy Get Countries",
    "_postman_id": "24b8f137-caba-4992-99bf-a8e6f333db45",
    "description": "Finds all Country.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "facd3a6a-0845-475c-9f53-5c97dbff0907",
          "name": "getCountriesCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "countries/:country_id"
              ],
              "variable": [
                {
                  "id": "country_id",
                  "value": "country_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Country by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ea18d87-2789-4277-9770-643e601e6cc5"
            }
          ]
        },
        {
          "id": "84d9f2e2-c665-4cb0-8ff3-9f169962e87b",
          "name": "getCountries",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/countries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all Country."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e0caf52-12b0-49ea-b82e-0c61f35ae32d"
            }
          ]
        }
      ]
    }
  ]
}