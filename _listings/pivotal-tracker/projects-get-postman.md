{
  "info": {
    "name": "Pivotal Tracker Get Projects",
    "_postman_id": "38efb26a-aecd-43a6-b4a3-a9555ad88d95",
    "description": "Retrieves all of the user's projects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "d70c3bbc-30d9-4ea1-98db-6ea831a9aff1",
          "name": "getProjectsProjectActivities",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/activities"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "occurred_since_date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the recent activity of a specific project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72cc66c1-0593-4227-bb71-994e00e04b3a"
            }
          ]
        },
        {
          "id": "143508e0-a0a3-42f8-bfe7-69bef92c5d25",
          "name": "getProjectsProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7091935a-115e-44de-b58b-7b447c5d1862"
            }
          ]
        },
        {
          "id": "6b6b1aa3-246f-4d86-8bf0-f8e7bb7275a4",
          "name": "getProjects",
          "request": {
            "url": "http://www.pivotaltracker.com/services/v3/projects",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all of the user's projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40fff5e5-05b9-4d15-8357-16dce88aa620"
            }
          ]
        }
      ]
    }
  ]
}