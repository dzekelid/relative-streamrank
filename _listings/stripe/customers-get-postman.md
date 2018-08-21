{
  "info": {
    "name": "Stripe Get Customers",
    "_postman_id": "6b949181-8f45-4f17-8027-c7465661f47e",
    "description": "Returns a list of your customers. The customers are returned sorted by creation date, with the most recent customers appearing first.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "customers",
      "item": [
        {
          "id": "19343184-7ac6-4dc7-9fd2-464e1e77feee",
          "name": "getCustomers",
          "request": {
            "url": "http://api.stripe.com/v1/customers?created=%7B%7D&email=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your customers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70162e49-0ac9-48aa-a2ec-fcfef1f41c35"
            }
          ]
        }
      ]
    }
  ]
}