{
  "info": {
    "name": "AWS EC2 API Cancel Conversion Task",
    "_postman_id": "79209d94-8b08-432a-975c-1ae852ceb499",
    "description": "Cancels an active conversion task.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bundle Task",
      "item": [
        {
          "id": "c00b0081-a4d5-4200-9fbf-79d4f186c5e8",
          "name": "cancelbundletask",
          "request": {
            "url": "http://example.com/api/?Action=CancelBundleTask?BundleId.N=BundleId.N&DryRun=DryRun&Filter.N=Filter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a bundling operation for an instance store-backed Windows instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13919b5c-cf7c-46c3-a844-89602f3ac327"
            }
          ]
        },
        {
          "id": "52c660a2-c4be-4391-94e8-075f67741496",
          "name": "describebundletasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeBundleTasks?DryRun=DryRun&InstanceId=InstanceId&SecurityGroupId.N=SecurityGroupId.N&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your bundling tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e27e1e7e-b00f-4345-906b-d83aa5d46571"
            }
          ]
        },
        {
          "id": "c03ac71d-b432-4de6-81e0-3d36cc45f90d",
          "name": "cancelconversiontask",
          "request": {
            "url": "http://example.com/api/?Action=CancelConversionTask",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an active conversion task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ae61fa7-3933-438c-a94a-44c2575bb03e"
            }
          ]
        }
      ]
    }
  ]
}