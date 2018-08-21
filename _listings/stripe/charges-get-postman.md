{
  "info": {
    "name": "Stripe Get Charges",
    "_postman_id": "4e68dc8c-6af9-4cd3-8fd4-da0fe0b7e379",
    "description": "Returns a list of charges you???ve previously created. The charges are returned in sorted order, with the most recent charges appearing first.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "charges",
      "item": [
        {
          "id": "9de30d47-cbb2-4cc2-8c61-afac9309a1a0",
          "name": "getCharges",
          "request": {
            "url": "http://api.stripe.com/v1/charges?created=%7B%7D&customer=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&source=%7B%7D&starting_after=%7B%7D&transfer_group=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of charges you???ve previously created"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a96ba0d-3ef6-48d1-bcdc-c2416ef886fb"
            }
          ]
        }
      ]
    }
  ]
}