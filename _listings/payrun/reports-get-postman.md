{
  "info": {
    "name": "Pay Run.IO Gets all reports",
    "_postman_id": "a469922c-3cba-452a-a94c-faaac45c4f09",
    "description": "Get links to all saved report definitions under authorised application",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "bf074da7-edd3-4d6e-b707-e4f00dc6dfc5",
      "name": "GetReportDefinitionsFromApplication",
      "request": {
        "url": "http://api.test.payrun.io/Reports",
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
        "description": "Get links to all saved report definitions under authorised application"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "9a564f04-0701-4165-9f08-c22673a2878e"
        }
      ]
    }
  ]
}