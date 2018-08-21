{
  "info": {
    "name": "Pivotal Tracker Get Activities",
    "_postman_id": "aafc2596-ab46-4c91-8971-52cb852fd38b",
    "description": "Retrieves the recent activity of all your projects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activities",
      "item": [
        {
          "id": "11a29ac2-2a35-452e-be67-587986c5773f",
          "name": "getActivities",
          "request": {
            "url": "http://www.pivotaltracker.com/services/v3/activities?limit=%7B%7D&newer_than_version=%7B%7D&occurred_since_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the recent activity of all your projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "299431b7-9787-4352-aeb2-d113a6ce5442"
            }
          ]
        }
      ]
    }
  ]
}