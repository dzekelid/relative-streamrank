{
  "info": {
    "name": "Sugar Sync  API Retrieving Workspace Information",
    "_postman_id": "b49ab299-a538-4ef7-adfc-b228c8adb8eb",
    "description": "To retrieve information about a workspace, an application submits an HTTP GET request to then          workspace resource that represents the workspace.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "28d80fcb-c7d1-404e-92ae-be615e8b1dbd",
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
              "id": "92b1e6d6-8932-4fe8-bcd7-609d1d9cb692"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "6b5fe566-eb55-472b-a0bf-eeb24b663249",
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
              "id": "26cc593c-ece8-4219-8561-49b2974e5950"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization",
      "item": [
        {
          "id": "c2b04c1b-8590-4675-a8e2-9fb8f6516190",
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
              "id": "f5f97e2c-cdd2-46e7-9963-1beae920a0ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "f7a8ee60-2f92-4fb6-8496-ae4dcb839f02",
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
              "id": "39276353-aac9-4b7c-8ed3-cb0bce263c40"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "19c94ada-b800-4e7b-a6e1-11e6ea89a364",
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
              "id": "bea531e7-4a10-475c-9b30-454768fa146c"
            }
          ]
        },
        {
          "id": "91db49e7-c036-4db7-9e93-1c9dc75f2243",
          "name": "uploading-file-data",
          "request": {
            "url": "http://api.sugarsync.com/file",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "An application can upload data to a file by issuing an HTTP PUT request to thenfile data resource that represents the data for the file.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2f5d6df-0841-45da-871f-9b31967b4364"
            }
          ]
        },
        {
          "id": "eafe0669-8b29-40b8-9fde-e6553cb85936",
          "name": "retrieving-file-information",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a file, an application submits an HTTP GET request to then          file resource that represents the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffbedcce-5d08-496b-970a-c338ab96222f"
            }
          ]
        },
        {
          "id": "76fa5dd2-b63b-4a31-b5c8-2c004362b837",
          "name": "updating-file-information",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
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
            "description": "An application can update various attributes of a file by issuing an HTTP PUT request to the URL thatnrepresents the file resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the file. Upon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9ddc881-789e-48ba-8009-6607fbdecf93"
            }
          ]
        },
        {
          "id": "2373ef61-1ccd-4ee2-b064-588e2c549be9",
          "name": "creating-a-new-file-version",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "nAn application can create a new version of a file by submitting an HTTP POST request to the URL that represents the version history. The version history URL is returned in the &lt;versions&gt; element whenn retrieving information about a file.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca2d0150-b98d-4059-a78a-a30c265085d9"
            }
          ]
        },
        {
          "id": "24464279-b107-4852-8843-6b6751018dfb",
          "name": "deleting-a-file",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An application can permanently delete a file by issuing an HTTP DELETE request to the URL of thenfile resource.nIts a good idea to precede DELETE requests like this with a caution note in your applications user interface.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bd27e2f-605c-4de7-8ed4-1f3bde201ac0"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "1d85e488-8b39-4699-9cb2-7e9f21d74600",
          "name": "retrieving-folder-information",
          "request": {
            "url": "http://api.sugarsync.com/folder",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a folder, an application submits an HTTP GET request to then          folder resource that represents the folder."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "980c6438-41c3-4254-bce8-66e85c3bd7db"
            }
          ]
        },
        {
          "id": "df2691bd-32c5-48ea-b609-b3111b808503",
          "name": "retrieving-folder-contents",
          "request": {
            "url": "http://api.sugarsync.com/folder/?max=%7B%7D&order=%7B%7D&start=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve the contents of a folder, an application submits an HTTP GET request to the URLn          that represents the folder contents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd77e044-c8af-415b-97d1-8baa8463557a"
            }
          ]
        },
        {
          "id": "daf57509-a0a3-4330-afbf-151fd9ece852",
          "name": "updating-folder-information",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
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
            "description": "An application can update various attributes of a folder by issuing an HTTP PUT request to the URL thatnrepresents the folder resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the folder. Upon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae51c42a-e878-4d2f-ab40-d35e625fd5db"
            }
          ]
        },
        {
          "id": "5b86d1ad-ff1c-4bf8-8a2e-de5a61585d9f",
          "name": "creating-a-folder",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
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
            "description": "An application can create a folder within another folder by issuing an HTTP POST request to the URL ofnthe containing folder resource.nIn addition, the application needs to provide as input, XML that identifies the display name of the folder to be created.nNote that an application can create a folder only within another folder, and not directly in a workspace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67c02918-ca7d-4f39-b371-8112a2f2a83d"
            }
          ]
        },
        {
          "id": "2ca05d53-2dd2-43c9-900a-838133f4a662",
          "name": "deleting-a-folder",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An application can permanantly delete a folder by issuing an HTTP DELETE request to the URL of thenfolder resource.nIts a good idea to precede DELETE requests like this with a caution note in your applications user interface.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "355dcb32-3f28-46ba-9906-3fc22c16c965"
            }
          ]
        }
      ]
    },
    {
      "name": "ReceivedShare",
      "item": [
        {
          "id": "31d2e55c-e21a-4742-9aaa-a238879b9056",
          "name": "retrieving-received-share-information",
          "request": {
            "url": "http://api.sugarsync.com/receivedShare/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a received share (that is, a shared folder owned by another user and to whichnthis user has been granted access privileges by the owner), an application submits an HTTP GET request to the URLnthat represents the received share resource. The URL is referenced in the &lt;receivedShare&gt; element for the received share in the received shares list.nSee Retrieving the Received Shares List."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d95a09a-4682-4e74-a1b1-2c76a6908a5b"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "573ad3b5-cc17-4f21-a118-3010b75190cf",
          "name": "retrieving-user-information",
          "request": {
            "url": "http://api.sugarsync.com/user?max=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a SugarSync user, an application submits an HTTP GET request to thenuser resource that represents the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff3c2b6f-70c9-47f3-9158-02fafa57968f"
            }
          ]
        },
        {
          "id": "c6088814-8eac-495e-a8e9-fbc9bd21e81d",
          "name": "retrieving-received-shares-list",
          "request": {
            "url": "http://api.sugarsync.com/user/?max=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "One of the elements in the representation of a user resource isn&lt;receivedShares&gt;.nThe element contains a link to a list that describes the shared folders that are owned by other users and to which this user has been granted access privileges by those owners. For example:nnn&lt;?xml version=1.0 encoding=UTF-8?&gt;n&lt;user&gt;n  ...n  &lt;receivedShares&gt;https://api.sugarsync.com/user/5664947/receivedShares/contents&lt;/receivedShares&gt;n  ...n&lt;/user&gt;nnn          To retrieve the list, an application submits an HTTP GET request to the link in the &lt;receivedShares&gt;nelement.nn         Requestnn          URLn          The URL that represents the received shares list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3446872-b93f-4618-8e70-a9ea6b378898"
            }
          ]
        }
      ]
    },
    {
      "name": "Workspace",
      "item": [
        {
          "id": "241828f4-0191-4d8b-86fa-ff5043d2e739",
          "name": "retrieving-workspace-information",
          "request": {
            "url": "http://api.sugarsync.com/workspace",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a workspace, an application submits an HTTP GET request to then          workspace resource that represents the workspace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60da68a5-5bca-4438-b2d9-20ebc7fa4c67"
            }
          ]
        }
      ]
    }
  ]
}