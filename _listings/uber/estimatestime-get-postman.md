{
  "info": {
    "name": "Uber Time Estimates",
    "_postman_id": "abb5b42d-a870-4c4d-8ce7-77ff5b228990",
    "description": "The Time Estimates endpoint returns ETAs for all products offered at a given location, with the responses expressed as integers in seconds. We recommend that this endpoint be called every minute to provide the most accurate, up-to-date ETAs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transportation",
      "item": [
        {
          "id": "737395f2-f405-4293-aa0c-16079c3ebc42",
          "name": "the-time-estimates-endpoint-returns-etas-for-all-products-offered-at-a-given-location-with-the-respo",
          "request": {
            "url": "http://api.uber.com/v1/estimates/time?customer_uuid=%7B%7D&product_id=%7B%7D&start_latitude=%7B%7D&start_longitude=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Time Estimates endpoint returns ETAs for all products offered at a given location, with the responses expressed as integers in seconds"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b1f05d8-002a-4a12-a268-417818e79f71"
            }
          ]
        }
      ]
    }
  ]
}