{
  "info": {
    "name": "Stripe Get Orders",
    "_postman_id": "704fca5b-303f-4725-8bcd-6a6f0b5c5f1d",
    "description": "Returns a list of your orders. The orders are returned sorted by creation date, with the most recently created orders appearing first.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "orders",
      "item": [
        {
          "id": "76507ee6-f969-4a3c-a069-233fc803d332",
          "name": "getOrders",
          "request": {
            "url": "http://api.stripe.com/v1/orders?created=%7B%7D&customer=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&ids=%7B%7D&limit=%7B%7D&starting_after=%7B%7D&status=%7B%7D&status_transitions=%7B%7D&upstream_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your orders"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e06e3615-d1b0-4e6c-8e7a-b51c00c9717e"
            }
          ]
        }
      ]
    }
  ]
}