{
  "info": {
    "name": "Sugar Sync  API Retrieving File Data",
    "_postman_id": "9b90529b-eeec-44b0-af7a-5c4fc59ab892",
    "description": "To retrieve file data, an application submits an HTTP GET request to then          file data resource that represents the data for the file.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "cb8409a4-4696-4132-b7b3-a50b803c2032",
          "name": "retrieving-album-information",
          "request": {
            "url": "http://api.sugarsync.com/album/?max=%7B%7D&order=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about an album, an application submits an HTTP GET request to then          album resource that represents the album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce177a1b-03f1-42da-bf0c-41bebf95a7af"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "16f35073-c757-47b6-9840-dbfe072c900a",
          "name": "creating-a-refresh-token",
          "request": {
            "url": "http://api.sugarsync.com/app-authorization",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application needs to be authorized to access a users SugarSync resources through the Platform API.nTo do that, the app needs to create a refresh token. When a user first runs the application, it creates a refresh tokennby submitting a POST request that includes the users credentials to the API.nIf the request is successful, the SugarSync service grants the application permission to access the users account and returns a refresh token.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3b6c3c4-02db-4451-960a-ea4dbe85019e"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization",
      "item": [
        {
          "id": "d7979685-8bb1-437e-9939-453e5dcc4e9c",
          "name": "creating-an-access-token",
          "request": {
            "url": "http://api.sugarsync.com/authorization",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application needs to be authorized to access a users SugarSync resources through the Platform API. To do that,nthe app needs to create an access token, which allows the app to access files, folders,nand other resources within a users account. After the token is created, the app needs to specify it in the HTTP request header when it makes a request through the API to access a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "379acb0e-d81e-476c-a27f-b0f8ce4178f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "6276e7cb-827e-48d3-960f-942bb3447692",
          "name": "retrieving-contact-information",
          "request": {
            "url": "http://api.sugarsync.com/contact/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A contact represents another SugarSync user who has shared a folder or folders with this user.n          To retrieve information about a contact, an application submits an HTTP GET request to then          contact resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70f98a73-ec2c-4a2b-a239-383ed8781645"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "44d62b51-c460-46d9-9bd1-3fc2c4cdb3aa",
          "name": "retrieving-file-data",
          "request": {
            "url": "http://api.sugarsync.com/file",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve file data, an application submits an HTTP GET request to then          file data resource that represents the data for the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5262aaa5-b7ac-499b-9b49-b196e88ef074"
            }
          ]
        }
      ]
    }
  ]
}