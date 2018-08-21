{
  "info": {
    "name": "Youtube Get Channels",
    "_postman_id": "728525fe-5e58-4624-b39c-ffb343cb6830",
    "description": "Returns a collection of zero or more channel resources that match the request criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "channels",
      "item": [
        {
          "id": "4e104a27-3f34-4b03-865e-32296c937ca6",
          "name": "getChannels",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/channels?categoryId=%7B%7D&forUsername=%7B%7D&hl=%7B%7D&id=%7B%7D&managedByMe=%7B%7D&maxResults=%7B%7D&mine=%7B%7D&mySubscribers=%7B%7D&onBehalfOfContentOwner=%7B%7D&pageToken=%7B%7D&part=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of zero or more channel resources that match the request criteria"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b5b42f4-e562-4c25-a6e3-b512ad3bf423"
            }
          ]
        }
      ]
    }
  ]
}