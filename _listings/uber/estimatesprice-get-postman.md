{
  "info": {
    "name": "Uber Price Estimates",
    "_postman_id": "1412e098-65f8-4a63-9912-f3303ab47b69",
    "description": "The Price Estimates endpoint returns an estimated price range for each product offered at a given location. The price estimate is provided as a formatted string with the full price range and the localized currency symbol.<br><br>The response also includes low and high estimates, and the [ISO 4217](http://en.wikipedia.org/wiki/ISO_4217) currency code for situations requiring currency conversion. When surge is active for a particular product, its surge_multiplier will be greater than 1, but the price estimate already factors in this multiplier.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transportation",
      "item": [
        {
          "id": "18fa64a5-869b-4e8c-bc89-e5680a56f0d2",
          "name": "the-price-estimates-endpoint-returns-an-estimated-price-range-for-each-product-offered-at-a-given-lo",
          "request": {
            "url": "http://api.uber.com/v1/estimates/price?end_latitude=%7B%7D&end_longitude=%7B%7D&start_latitude=%7B%7D&start_longitude=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Price Estimates endpoint returns an estimated price range for each product offered at a given location"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39129eb8-ae92-4210-8015-559426b66d83"
            }
          ]
        }
      ]
    }
  ]
}