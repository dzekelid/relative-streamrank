{
  "info": {
    "name": "Stripe Get Payments",
    "_postman_id": "083167b1-2013-49ef-80f6-3a55d370e0a7",
    "description": "Get Payments",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "payments",
      "item": [
        {
          "id": "33123044-c01b-40d1-a779-6af2a35b4ed4",
          "name": "getPayments",
          "request": {
            "url": "http://api.stripe.com/v1/payments?customer=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D&transfer_group=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Payments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9f5cf6f-eae0-452d-9934-e1cb3fee7165"
            }
          ]
        }
      ]
    }
  ]
}