{
  "info": {
    "name": "Click Meter Retrieve a list of conversions",
    "_postman_id": "0915dead-5c49-41a3-84f9-075979460eae",
    "description": "Retrieve a list of conversions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Aggregated",
      "item": [
        {
          "id": "e1983a36-c1fd-4d3a-8bca-8925f48f5327",
          "name": "getAggregatedSummaryConversions",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/aggregated/summary/conversions?fromDay=%7B%7D&limit=%7B%7D&offset=%7B%7D&sortBy=%7B%7D&sortDirection=%7B%7D&status=%7B%7D&textSearch=%7B%7D&timeFrame=%7B%7D&toDay=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve statistics about a subset of conversions for a timeframe with conversions data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "488f65fb-b288-460c-8332-d115bf97ab08"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversions",
      "item": [
        {
          "id": "78cffaea-b53c-4c53-8a05-a178f5ca335e",
          "name": "getConversions",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/conversions?createdAfter=%7B%7D&createdBefore=%7B%7D&limit=%7B%7D&offset=%7B%7D&status=%7B%7D&textSearch=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of conversions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9afe26a0-084f-462a-9264-d30430200886"
            }
          ]
        }
      ]
    }
  ]
}