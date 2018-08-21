{
  "info": {
    "name": "Pay Run.IO Get all PayRun jobs",
    "_postman_id": "e410e015-8df0-430b-bc9d-35fc97aa1821",
    "description": "Gets all the pay run jobs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "DPJobs",
      "item": [
        {
          "id": "f2a8d86b-3028-4e53-b4c4-02e5d9317a2a",
          "name": "GetDpsJobs",
          "request": {
            "url": "http://api.test.payrun.io/Jobs/Dps",
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the DPS jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e46a23f-2e2d-4740-86b4-3021627d839b"
            }
          ]
        }
      ]
    },
    {
      "name": "PayRun",
      "item": [
        {
          "id": "c7f383cc-907d-4fe6-a8c2-f79a6a4d9a18",
          "name": "GetPayRunJobs",
          "request": {
            "url": "http://api.test.payrun.io/Jobs/PayRuns",
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pay run jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd797b0d-e802-4bac-a021-bec883630b44"
            }
          ]
        }
      ]
    }
  ]
}