{
  "info": {
    "name": "Youtube Get Comments",
    "_postman_id": "46fad7b0-d5a3-45a5-b558-2e8976c75bc7",
    "description": "Returns a list of comments that match the API request parameters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "comments",
      "item": [
        {
          "id": "9cfd9263-3b0e-4110-b010-d5f4e165e450",
          "name": "getComments",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/comments?id=%7B%7D&maxResults=%7B%7D&pageToken=%7B%7D&parentId=%7B%7D&part=%7B%7D&textFormat=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of comments that match the API request parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60560596-f773-48e9-9ccd-df9b6f530eb4"
            }
          ]
        }
      ]
    }
  ]
}