{
  "info": {
    "name": "SendGrid Get Campaigns",
    "_postman_id": "9450bf13-40b2-4147-8d88-2c8ee47d52c0",
    "description": "**This endpoint allows you to retrieve a list of all of your campaigns.**\n\nReturns campaigns in reverse order they were created (newest first).\n\nReturns an empty array if no campaigns exist.\n\nFor more information:\n\n* [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "3f505e9c-f618-41fa-bd02-dadb2e0a238c",
          "name": "GET_campaigns",
          "request": {
            "url": "http://api.sendgrid.com/v3/campaigns?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all of your campaigns"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12d6f011-3d26-4951-ad69-d977efa22cd5"
            }
          ]
        }
      ]
    }
  ]
}