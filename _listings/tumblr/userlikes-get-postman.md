{
  "info": {
    "name": "Tumblr Get User Likes",
    "_postman_id": "ed9512e2-8d7e-4c35-a06e-94ba9818d641",
    "description": "Use this method to retrieve the liked posts that match the OAuth credentials submitted with the request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "125ba571-0123-405a-9411-ba43d870b8ee",
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
              "id": "4c35ca92-b866-4d86-be85-e90d18de3735"
            }
          ]
        },
        {
          "id": "6427e526-27d4-4de6-9c87-0900dce4bb8e",
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
              "id": "a969c597-67d1-47ca-83c6-16343e9c1198"
            }
          ]
        },
        {
          "id": "28aab3c3-6157-4b6b-86e5-d7c4eeef48d3",
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
              "id": "1b7c0602-86a6-4613-81eb-65cdacc88a07"
            }
          ]
        },
        {
          "id": "a5e8f407-88e1-4d83-9b61-8310a9e4e724",
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
              "id": "2f4f8aa0-97cb-405b-87e0-e0f763cba2a5"
            }
          ]
        },
        {
          "id": "5a92eceb-2cdf-4046-bd9e-a45887913f5e",
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
              "id": "f105325c-502b-47f6-ae1d-c235f8c91d26"
            }
          ]
        },
        {
          "id": "8c41d1f0-0658-424a-afc2-00a67798c962",
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
              "id": "293c3c7f-3d6a-4b19-831d-560c6b80bf4f"
            }
          ]
        },
        {
          "id": "5f94c50b-c894-4e22-b968-d4670f871a7f",
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
              "id": "8139258a-b143-4774-aa97-48e0fcfb37f6"
            }
          ]
        },
        {
          "id": "6fb228a6-44bb-401f-bf91-5c165daca68c",
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
              "id": "a10f99de-dc10-4be7-8852-648626f39c33"
            }
          ]
        },
        {
          "id": "59a18ffd-400e-4bd1-8018-4a63cf8c958d",
          "name": "blog.base_hostname.post.edit.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/edit"
              ],
              "query": [
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
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
            "description": "Edits a blog post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5867aad-15c7-4c17-954a-cac0d94feb62"
            }
          ]
        },
        {
          "id": "1cc7d5c3-f150-4058-9cb7-f4343aad2056",
          "name": "blog.base_hostname.post.reblog.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/reblog"
              ],
              "query": [
                {
                  "key": "comment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reblog_key",
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
            "description": "Reblogs a post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e7c59e0-dbc2-4ac4-af2e-a30f2ada14a3"
            }
          ]
        },
        {
          "id": "ac737357-5f00-4c8b-9fd0-7443392db99e",
          "name": "blog.base_hostname.post.delete.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/delete"
              ],
              "query": [
                {
                  "key": "id",
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
            "description": "Deletes a post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "393a26f2-b3da-416d-8c9b-d507c3a67140"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "dafc1948-9afc-425f-a116-1fada8f18cc7",
          "name": "user.dashboard.get",
          "request": {
            "url": "http://api.tumblr.com/v2/user/dashboard?limit=%7B%7D&offset=%7B%7D&since_id=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this method to retrieve the dashboard that matches the OAuth credentials submitted with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c19802fa-c265-4476-a1bc-89c8ececc277"
            }
          ]
        },
        {
          "id": "7e46d617-cd25-4af5-a73f-02eae8f71011",
          "name": "user.likes.get",
          "request": {
            "url": "http://api.tumblr.com/v2/user/likes?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this method to retrieve the liked posts that match the OAuth credentials submitted with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "376911a3-355b-4445-aac4-89ddad333f67"
            }
          ]
        }
      ]
    }
  ]
}