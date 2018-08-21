{
  "info": {
    "name": "Stripe Get Coupons",
    "_postman_id": "ab8116fd-2b60-41db-ac8e-d13d5c1e53e0",
    "description": "Returns a list of your coupons.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "coupons",
      "item": [
        {
          "id": "99a845fd-726b-43c4-96a6-b3ee12cdcacd",
          "name": "getCoupons",
          "request": {
            "url": "http://api.stripe.com/v1/coupons?created=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your coupons"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a90751a-1238-4f69-b912-8a87c00465e3"
            }
          ]
        }
      ]
    }
  ]
}