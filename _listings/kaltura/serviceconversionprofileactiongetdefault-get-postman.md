{
  "info": {
    "name": "Kaltura VPaaS Get Service Conversionprofile Action Getdefault",
    "_postman_id": "c64c04a9-afe7-4f19-ba0c-0c0d5c548354",
    "description": "Get the partner's default conversion profile",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "4bcb075e-322b-4078-8e3f-a1c92dfe0bb3",
          "name": "captionAsset.setAsDefault",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/caption_captionasset/action/setAsDefault?captionAssetId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Markss the caption as default and removes that mark from all other caption assets of the entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e60b98f-205b-4446-99b5-ac74e546edde"
            }
          ]
        },
        {
          "id": "57914649-c419-481d-b7f0-530c8b7a3952",
          "name": "conversionProfile.getDefault",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/conversionprofile/action/getDefault?No Name=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the partner's default conversion profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0319702e-ea05-465d-b939-df99d14c59cf"
            }
          ]
        }
      ]
    }
  ]
}