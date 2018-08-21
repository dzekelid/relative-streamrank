{
  "info": {
    "name": "Stripe Get Balance",
    "_postman_id": "cce70745-9e8c-42cb-956c-4935044f0da8",
    "description": "Retrieves the current account balance, based on the authentication that was used to make the request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "balance",
      "item": [
        {
          "id": "7000045e-260e-4ad4-92db-12b7bc8afd8d",
          "name": "getBalance",
          "request": {
            "url": "http://api.stripe.com/v1/balance?expand=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current account balance, based on the authentication that was used to make the request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71e2a291-a1b6-4866-b95c-510778a4c0ac"
            }
          ]
        }
      ]
    }
  ]
}