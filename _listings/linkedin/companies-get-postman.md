{
  "info": {
    "name": "LinkedIn Get Companies",
    "_postman_id": "fcca27cf-04d9-4dbd-a177-43611e51bc41",
    "description": "Get companies",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Companies",
      "item": [
        {
          "id": "ece532c1-bb5e-4504-b801-d812767a9f70",
          "name": "postCompaniesUpdatesKeyUpdateKeyUpdateCommentsAsCompany",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.linkedin.com",
              "path": [
                "v1",
                "companies/:id/updates/key=:update-key/update-comments-as-company/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "update-key",
                  "value": "update-key",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post companies  updates key update key update comments as company"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f440a75c-2323-4513-9674-f0cdda19b0e7"
            }
          ]
        },
        {
          "id": "017ea4db-d5b7-4b1f-aaef-5a54bef0e5a8",
          "name": "getCompaniesIsCompanyShareEnabled",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.linkedin.com",
              "path": [
                "v1",
                "companies/:id/is-company-share-enabled"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get companies  is company share enabled"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4feec882-f012-491a-8f2a-f391f7618b83"
            }
          ]
        },
        {
          "id": "cdef47b7-82a2-4f9f-ba4c-3dcef87bfeb0",
          "name": "getCompaniesRelationToViewerIsCompanyShareEnabled",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.linkedin.com",
              "path": [
                "v1",
                "companies/:id/relation-to-viewer/is-company-share-enabled"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get companies  relation to viewer is company share enabled"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52ea3bcf-a701-4af2-8f10-d13c6b0cd4b0"
            }
          ]
        },
        {
          "id": "db82313e-9a11-48ce-8e90-3f71a86ad3eb",
          "name": "getCompanies",
          "request": {
            "url": "http://api.linkedin.com/v1/companies/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get companies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e920e16f-eacd-4324-8097-daacea545818"
            }
          ]
        }
      ]
    }
  ]
}