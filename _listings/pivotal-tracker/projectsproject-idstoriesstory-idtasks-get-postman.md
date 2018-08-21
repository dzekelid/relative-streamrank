{
  "info": {
    "name": "Pivotal Tracker Get Projects Project Stories Story Tasks",
    "_postman_id": "58f7bdf1-f42c-4bb5-b24c-bf5e3b60abe5",
    "description": "Get projects project stories story tasks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "47d05012-9759-49b8-9a9c-ecd2504ad7eb",
          "name": "getProjectsProjectStoriesStoryTasksTask",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks/:TASK_ID"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "STORY_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "TASK_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get projects project stories story tasks task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a09068a-0a95-4390-ab7d-6609c04d9bb9"
            }
          ]
        },
        {
          "id": "1970120c-08a7-49c8-bbf8-e96f0fe5b58c",
          "name": "putProjectsProjectStoriesStoryTasksTask",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks/:TASK_ID"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "STORY_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "TASK_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Put projects project stories story tasks task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c7ba2dc-9d43-496e-9cf8-3f1af9b29ea4"
            }
          ]
        },
        {
          "id": "123a8207-432c-4c96-9f4a-b51f1ceecaf5",
          "name": "deleteProjectsProjectStoriesStoryTasksTask",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks/:TASK_ID"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "STORY_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "TASK_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete projects project stories story tasks task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47b63a11-b39e-4f7a-b20a-53f7f5c7aef9"
            }
          ]
        },
        {
          "id": "a9d0ff34-c798-4772-9d8a-a75a739c3f38",
          "name": "getProjectsProjectStoriesStoryTasks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "STORY_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get projects project stories story tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d56066fd-f874-4a99-9921-cfab520ba676"
            }
          ]
        }
      ]
    }
  ]
}