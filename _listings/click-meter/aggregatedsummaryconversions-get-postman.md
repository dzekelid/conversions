{
  "info": {
    "name": "Click Meter Retrieve statistics about a subset of conversions for a timeframe with conversions data",
    "_postman_id": "1e4d09f4-2cce-4970-ac7f-f02d2a7e7fa5",
    "description": "Retrieve statistics about a subset of conversions for a timeframe with conversions data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Aggregated",
      "item": [
        {
          "id": "80ea8433-3272-457a-a889-36cd4b3bf3bd",
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
              "id": "c3ac941b-0475-4f99-adbb-6e47ea59aa9c"
            }
          ]
        }
      ]
    }
  ]
}