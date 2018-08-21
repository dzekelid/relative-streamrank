{
  "info": {
    "name": "Youtube Get Groups",
    "_postman_id": "7df8d0ef-720e-4030-9480-3ecaf767b81f",
    "description": "Returns a collection of groups that match the API request parameters. For example, you can retrieve all groups that the authenticated user owns, or you can retrieve one or more groups by their unique IDs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "2f6112f8-c11c-46bb-9ca9-8a1e43f021fa",
          "name": "getGroups",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/groups?id=%7B%7D&mine=%7B%7D&onBehalfOfContentOwner=%7B%7D&pageToken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of groups that match the API request parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66dd2bbd-b4a2-45ea-994d-01c1d3f27208"
            }
          ]
        }
      ]
    }
  ]
}