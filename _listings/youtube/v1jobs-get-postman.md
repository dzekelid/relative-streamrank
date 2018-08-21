{
  "info": {
    "name": "Youtube Get Jobs",
    "_postman_id": "dc78ac0e-a0c7-4081-aca7-5a0a74447def",
    "description": "Lists jobs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "v1",
      "item": [
        {
          "id": "3c27d95a-0ce3-46bd-b315-c61408b93a59",
          "name": "getV1Jobs",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/v1/jobs?includeSystemManaged=%7B%7D&onBehalfOfContentOwner=%7B%7D&pageSize=%7B%7D&pageToken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "164bdace-f82a-47e4-aa84-0005721e9f1d"
            }
          ]
        }
      ]
    }
  ]
}