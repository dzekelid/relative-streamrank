{
  "info": {
    "name": "Pivotal Tracker Get Projects Project Stories",
    "_postman_id": "38385283-cc7d-4aab-b309-03c187e2794a",
    "description": "Retrieves all stories for a project, or those matching filter(s)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "f8117c64-1b4b-4645-b3ef-346cec8bf9dc",
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
              "id": "f9f5f852-9b7d-4177-8a13-07d5c5fbe2a6"
            }
          ]
        },
        {
          "id": "29f58f51-670a-4707-bc0f-be509351124f",
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
              "id": "5156c283-cb78-420e-b6ae-2d09d81c7939"
            }
          ]
        },
        {
          "id": "cce11ad9-e3b0-415b-b14b-7e2351552a46",
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
              "id": "a4389f01-e169-44bc-95d2-140dfaced8ad"
            }
          ]
        },
        {
          "id": "eebdf1d4-486e-42cf-8c0b-87cfb74fa0ac",
          "name": "postProjects",
          "request": {
            "url": "http://www.pivotaltracker.com/services/v3/projects",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa74b0b4-e30f-4940-9f38-72bb5ecff564"
            }
          ]
        },
        {
          "id": "e5220ffe-5e9d-4203-8151-b8dfc5d081a3",
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
              "id": "57b7bb39-5f1e-4fbd-b413-dc64db5d0717"
            }
          ]
        },
        {
          "id": "3171d328-d1c2-418c-ab19-6162907bfb41",
          "name": "postProjectsProjectMemberships",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new membership to a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "167d7ca1-9825-4307-9c8c-abe92836b1e4"
            }
          ]
        },
        {
          "id": "a4fb8063-d4b0-429c-ae46-8618eb8b6723",
          "name": "getProjectsProjectMembershipsMembership",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/memberships/:MEMBERSHIP_ID"
              ],
              "variable": [
                {
                  "id": "MEMBERSHIP_ID",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Retrieves information about a single membership."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9f4528b-a073-4760-8aa9-a9563d48d8ae"
            }
          ]
        },
        {
          "id": "68b9a0d4-3316-495e-8274-3574a32d9c93",
          "name": "deleteProjectsProjectMembershipsMembership",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/memberships/:MEMBERSHIP_ID"
              ],
              "variable": [
                {
                  "id": "MEMBERSHIP_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete projects project memberships membership."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3cca4b6-949e-4dd5-831e-69893395731c"
            }
          ]
        },
        {
          "id": "be1b524e-4d11-4902-9a71-1d53e328b6a0",
          "name": "getProjectsProjectIterations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/iterations"
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
            "description": "Retrieves all iterations, with stories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56b700fd-232c-4187-85a2-ef00c5357990"
            }
          ]
        },
        {
          "id": "9fb17379-2326-4ee1-921d-ced2fdc5d283",
          "name": "getProjectsProjectIterationsDone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/iterations/done"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
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
            "description": "Retrieves iterations from the \"done\" group, with stories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db80ea76-cd64-4d8a-8b04-ff5fbcccf9fd"
            }
          ]
        },
        {
          "id": "fb1970a0-de3d-4e0a-9398-05e394923b77",
          "name": "getProjectsProjectIterationsCurrent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/iterations/current"
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
            "description": "Retrieves iterations from the \"current\" group, with stories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80967a52-a677-4ff1-850b-7d8fbdd7a55f"
            }
          ]
        },
        {
          "id": "a08c36cd-82ca-46e4-9256-0a39aacac7b7",
          "name": "getProjectsProjectIterationsBacklog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/iterations/backlog"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
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
            "description": "Retrieves iterations from the \"backlog\" group, with stories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e23b95e9-8fef-455e-974d-0cbb54e392a1"
            }
          ]
        },
        {
          "id": "2af78996-39dc-42b5-b521-4459548728d9",
          "name": "getProjectsProjectIterationsCurrentBacklog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/iterations/current_backlog"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
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
            "description": "Retrieves iterations from the \"current\" and \"backlog\" groups, with stories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58025199-a41b-4fda-b13d-036553c15737"
            }
          ]
        },
        {
          "id": "e8684f64-2623-409a-97e7-dc708e8a66b3",
          "name": "getProjectsProjectStoriesStory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID"
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
            "description": "Retrieves information about a single story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d3aef55-6329-42b0-8f8d-8e42148cb87f"
            }
          ]
        },
        {
          "id": "0d71e295-e658-4d74-8c7c-5e22c10b69cf",
          "name": "putProjectsProjectStoriesStory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID"
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Put projects project stories story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "210174c2-11f4-440a-a988-90e07bcaaacc"
            }
          ]
        },
        {
          "id": "492c8ec9-2867-4928-9127-33b13bce6b51",
          "name": "deleteProjectsProjectStoriesStory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete projects project stories story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35498507-b782-4297-8e69-3c497cadbbce"
            }
          ]
        },
        {
          "id": "1e601479-4aa1-4936-a9ac-1b312aca4b3f",
          "name": "getProjectsProjectStories",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
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
            "description": "Retrieves all stories for a project, or those matching filter(s)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6f1ffd4-c103-4bfb-8fb3-36602a56cf1a"
            }
          ]
        }
      ]
    }
  ]
}