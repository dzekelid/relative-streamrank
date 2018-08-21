{
  "info": {
    "name": "Stripe Get Refunds",
    "_postman_id": "8bfb4edb-ae7f-44ac-8a99-5862cabbd3c9",
    "description": "Returns a list of all refunds you???ve previously created. The refunds are returned in sorted order, with the most recent refunds appearing first. For convenience, the 10 most recent refunds are always available by default on the charge object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "refunds",
      "item": [
        {
          "id": "3a4b60d7-f6ed-4495-93a0-e29d6d8df8aa",
          "name": "getRefunds",
          "request": {
            "url": "http://api.stripe.com/v1/refunds?charge=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all refunds you???ve previously created"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43226292-4235-4073-82fc-96e2238a4a78"
            }
          ]
        }
      ]
    }
  ]
}