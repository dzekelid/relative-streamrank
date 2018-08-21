{
  "info": {
    "name": "OpenDataSoft Get Pages",
    "_postman_id": "eefd7ed8-c80d-43b1-bfa0-a778c1826dbe",
    "description": "List of all pages from this portal.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pages",
      "item": [
        {
          "id": "e52431c3-60c4-431b-9480-e8c3949cf5d1",
          "name": "getPages",
          "request": {
            "url": "http://public.opendatasoft.com/api/v2/pages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of all pages from this portal."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dfa3634-a661-4a45-a34c-18f035581fde"
            }
          ]
        }
      ]
    }
  ]
}