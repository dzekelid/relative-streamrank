{
  "info": {
    "name": "Instagram Instagram User",
    "_postman_id": "123a9d5a-4e16-485a-98fa-c77524b6236f",
    "description": "Instagram User",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instagram",
      "item": [
        {
          "id": "459fc488-cf9b-42d9-9d63-dcc0c5b225fb",
          "name": "getInstagramMediaComments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-media-id&#125;/comments?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram Media Comments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddfcb699-9774-462b-a067-893ef74eba14"
            }
          ]
        },
        {
          "id": "b9317de1-c35f-4ba7-8860-473e38f05d8c",
          "name": "getInstagramUser",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-user-id&#125;?followed_by_countint32=followed_by_countint32&follow_countint32=follow_countint32&has_profile_picturebool=has_profile_picturebool&idnumeric string=idnumeric%20string&is_privatebool=is_privatebool&is_publishedbool=is_publishedbool&media_countint32=media_countint32&profile_picstring=profile_picstring&usernamestring=usernamestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77d108da-2997-4fee-8ab3-7ff342fc767d"
            }
          ]
        }
      ]
    }
  ]
}