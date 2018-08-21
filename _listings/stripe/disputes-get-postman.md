{
  "info": {
    "name": "Stripe Get Disputes",
    "_postman_id": "b9adc746-f8a6-4b8a-b5d0-af5294c37f6e",
    "description": "Returns a list of your disputes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "disputes",
      "item": [
        {
          "id": "e2991ade-d9f9-4535-8d77-a24465d2a0cf",
          "name": "getDisputes",
          "request": {
            "url": "http://api.stripe.com/v1/disputes?created=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your disputes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94161dfe-10fe-42b0-aa00-b27f74d909cc"
            }
          ]
        }
      ]
    }
  ]
}