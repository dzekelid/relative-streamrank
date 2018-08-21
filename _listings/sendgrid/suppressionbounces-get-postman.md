{
  "info": {
    "name": "SendGrid Get Suppression Bounces",
    "_postman_id": "e80b288e-974a-43df-9541-76d94f22b699",
    "description": "**This endpoint allows you to retrieve all of your bounces.**\n\nA bounced email is when the message is undeliverable and then returned to the server that sent it.  \n\nFor more information see: \n\n* [User Guide > Bounces](https://sendgrid.com/docs/User_Guide/Suppressions/bounces.html) for more information\n* [Glossary > Bounces](https://sendgrid.com/docs/Glossary/Bounces.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "8cf17cbf-ffe1-4236-a264-d55e4cedb6ff",
          "name": "suppression.bounces.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/suppression/bounces?end_time=%7B%7D&No Name=%7B%7D&start_time=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all of your bounces"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b6a705b-68e4-4c00-a5a4-c9bbaa394c00"
            }
          ]
        }
      ]
    }
  ]
}