{
  "info": {
    "name": "Tumblr Add Blog Base Hostname Add",
    "_postman_id": "03ab7469-8b5f-445e-9e55-f573a23689eb",
    "description": "Creates a new video blog post.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "b5cbff01-7321-4205-9b85-6bcb6290c316",
          "name": "blog.base_hostname.info.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/info"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method returns general information about the blog, such as the title, number of posts, and other high-level data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c0e9371-1c3d-4e2a-9874-21a479a7e671"
            }
          ]
        },
        {
          "id": "1fba8fda-c20d-4981-9369-23a9f025ac33",
          "name": "blog.base_hostname.avatar.size.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/avatar/:size"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                },
                {
                  "id": "size",
                  "value": "size",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a blog's avatar in one of 9 different sizes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "466eafe7-c861-48e7-9254-6093240bf060"
            }
          ]
        },
        {
          "id": "61cdc0c3-15e3-4cec-a1ce-e8b18a5985a1",
          "name": "blog.base_hostname.followers.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/followers"
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
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a blog's followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cfaf5d1-b4af-4a4d-8b66-ae9508b7a98c"
            }
          ]
        },
        {
          "id": "19eae642-b930-40ba-aad9-a6e38519a491",
          "name": "blog.base_hostname.posts.type.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/:type"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "notes_info",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reblog_info",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tag",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "type",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves published posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e630da6-ea07-40ce-b80d-05d52526f503"
            }
          ]
        },
        {
          "id": "6fbb7c69-36b4-4230-b060-2780a9fb5dfa",
          "name": "blog.base_hostname.posts.queue.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/queue"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves queued posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c40bea60-8b06-40ad-b240-b2f40e6531a5"
            }
          ]
        },
        {
          "id": "13982912-a83d-48a0-9bc7-268260576dcc",
          "name": "blog.base_hostname.posts.draft.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/draft"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves draft posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ff94410-c8dd-4d4e-b8f6-a1b3898f874a"
            }
          ]
        },
        {
          "id": "776602fe-28ee-43cd-a1f5-eaab005ad330",
          "name": "blog.base_hostname.posts.submission.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/submission"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves submission posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23ceae7d-d438-4d2f-8bb8-8669fb44ebee"
            }
          ]
        },
        {
          "id": "d8a3cf5a-1806-42f0-b64a-e5edfd845a3d",
          "name": "blog.base_hostname.post.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post"
              ],
              "query": [
                {
                  "key": "caption",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "data",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "embed",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new video blog post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7848b227-5e24-41fc-b1cf-c61dd6997359"
            }
          ]
        }
      ]
    }
  ]
}