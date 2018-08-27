{
  "info": {
    "name": "Kaltura VPaaS Get Service Conversionprofile Action Setasdefault",
    "_postman_id": "11ea7e40-4d05-4cff-94c2-17efa34bda92",
    "description": "Set Conversion Profile to be the partner default",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "700fc8a4-fd0a-417d-b9f4-3ba5204f0162",
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
              "id": "394d591a-08f6-403c-b518-f8382126d925"
            }
          ]
        },
        {
          "id": "a8e4dcd4-3446-4202-9439-8f526fd4e2ad",
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
              "id": "bf45bf0d-68fe-44d4-9792-5bc2a75736d2"
            }
          ]
        },
        {
          "id": "78539082-d975-4918-ae60-10deb970a31d",
          "name": "conversionProfile.setAsDefault",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/conversionprofile/action/setAsDefault?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Set Conversion Profile to be the partner default"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aca30080-d8c1-4db2-b8fd-45b9ac576606"
            }
          ]
        }
      ]
    }
  ]
}