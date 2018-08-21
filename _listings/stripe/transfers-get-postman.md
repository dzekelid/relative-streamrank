{
  "info": {
    "name": "Stripe Get Transfers",
    "_postman_id": "d7c08164-1822-4832-b604-4b382e7626b0",
    "description": "Returns a list of existing transfers sent to connected accounts. The transfers are returned in sorted order, with the most recently created transfers appearing first.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transfers",
      "item": [
        {
          "id": "f025b370-1e5e-402f-aa9f-f560917cff73",
          "name": "getTransfers",
          "request": {
            "url": "http://api.stripe.com/v1/transfers?created=%7B%7D&destination=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D&transfer_group=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of existing transfers sent to connected accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec91d0f1-5b8b-4bcb-8a3e-3e4ab2b86576"
            }
          ]
        }
      ]
    }
  ]
}