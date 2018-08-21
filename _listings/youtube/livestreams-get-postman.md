{
  "info": {
    "name": "Youtube Get Livestreams",
    "_postman_id": "1442809a-5a5b-465d-b5d3-a27143d9f1e2",
    "description": "Returns a list of video streams that match the API request parameters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "livestreams",
      "item": [
        {
          "id": "b5dbf63a-76a1-4e5f-9978-e192362e3b55",
          "name": "getLivestreams",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/liveStreams?id=%7B%7D&maxResults=%7B%7D&mine=%7B%7D&onBehalfOfContentOwner=%7B%7D&onBehalfOfContentOwnerChannel=%7B%7D&pageToken=%7B%7D&part=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of video streams that match the API request parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d97a149-3188-4396-8197-7f060d169fd2"
            }
          ]
        }
      ]
    }
  ]
}