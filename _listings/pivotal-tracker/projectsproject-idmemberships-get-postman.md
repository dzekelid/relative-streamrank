{
  "info": {
    "name": "Pivotal Tracker Get Projects Project Memberships",
    "_postman_id": "8cf4fa40-b8dc-4fe3-82b6-0ff93ebadd47",
    "description": "Retrieves all memberships for a project.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "e17068f8-3cd2-493a-8f59-08fcfb64ea68",
          "name": "getProjectsProjectMemberships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/memberships"
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
            "description": "Retrieves all memberships for a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2852583b-e167-470a-b48d-3b2e2fd2c581"
            }
          ]
        }
      ]
    }
  ]
}