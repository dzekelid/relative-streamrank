{
  "info": {
    "name": "Stripe Get Recipients",
    "_postman_id": "8b0aa4c9-98b7-4877-8b85-63cfd9013193",
    "description": "Returns a list of your recipients. The recipients are returned sorted by creation date, with the most recently created recipients appearing first.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recipients",
      "item": [
        {
          "id": "12162f19-7836-41a3-9654-9f9e0e5ba06a",
          "name": "getRecipients",
          "request": {
            "url": "http://api.stripe.com/v1/recipients?created=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D&type=%7B%7D&verified=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your recipients"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f79e3cb1-f029-438b-851c-c9209eb63146"
            }
          ]
        }
      ]
    }
  ]
}