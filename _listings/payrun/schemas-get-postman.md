{
  "info": {
    "name": "Pay Run.IO Get a list of all available schemas",
    "_postman_id": "25d33f0f-9e18-4f77-8a40-51d8d529b0f8",
    "description": "Returns a collection of links to all the available data object schemas",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "1a77d45d-88fc-4316-a8e5-506a95d13573",
          "name": "GetSchemas",
          "request": {
            "url": "http://api.test.payrun.io/Schemas",
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
            "description": "Returns a collection of links to all the available data object schemas"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d490308-8836-4529-a79c-124106c04a9f"
            }
          ]
        }
      ]
    }
  ]
}