{
  "info": {
    "name": "EU VAT API Convert a currency",
    "_postman_id": "2e8caf36-c805-43a2-ae01-c2003466d0c4",
    "description": "Convert a currency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "a3404d78-f8de-4841-9aac-808e21d29297",
          "name": "country_code_check",
          "request": {
            "url": "http://vatapi.com/v1/country-code-check?code=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Response-Type",
                "value": "{}",
                "description": "The default response type is application/json if you would like to receive an XML response then set this to XML",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a countries vat rates by its 2 digit country code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "281ed173-1f5d-4483-968c-93944961e4a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Convert",
      "item": [
        {
          "id": "af2b6a48-5f69-41ff-867c-1cf18478bcaa",
          "name": "currency_conversion",
          "request": {
            "url": "http://vatapi.com/v1/currency-conversion?amount=%7B%7D&currency_from=%7B%7D&currency_to=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Response-Type",
                "value": "{}",
                "description": "The default response type is application/json if you would like to receive an XML response then set this to XML",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Convert a currency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbc991a1-0c3e-4678-8dfb-ed377a737243"
            }
          ]
        }
      ]
    }
  ]
}