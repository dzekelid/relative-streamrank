{
  "info": {
    "name": "Stripe Get Events",
    "_postman_id": "cdf08b4d-6062-4a93-acd2-76590ca4954e",
    "description": "List events, going back up to 30 days.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "events",
      "item": [
        {
          "id": "12b7742b-e6c7-4ba6-87e6-2aba6c45ec6f",
          "name": "getEvents",
          "request": {
            "url": "http://api.stripe.com/v1/events?created=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D&type=%7B%7D&types=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List events, going back up to 30 days"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a8913e8-5ffd-46d5-a9cf-57f2d13d51b2"
            }
          ]
        }
      ]
    }
  ]
}