{
  "info": {
    "name": "Instagram Instagram Carousel",
    "_postman_id": "d84d9e37-0218-4f41-891c-9b2f68f193bf",
    "description": "Instagram Carousel",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instagram",
      "item": [
        {
          "id": "061aeadf-0e91-48d5-a24f-bc2201e001b3",
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
              "id": "0c5ffdef-e9a7-461c-abd6-3532833f1839"
            }
          ]
        },
        {
          "id": "5e37a7ad-9889-4194-824e-ba6df4fc8b1f",
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
              "id": "c6fc1e77-428e-48f9-9fc3-a437e1c0d7d2"
            }
          ]
        },
        {
          "id": "39c44f84-4058-467f-9103-372b5777370f",
          "name": "getInstagramUserAgencies",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-user-id&#125;/agencies?294=294",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram User Agencies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef3547a6-e0a1-4a95-b76c-9062f3f6e85d"
            }
          ]
        },
        {
          "id": "05e59fe7-5814-4b74-84d5-d86dfa10fadf",
          "name": "getInstagramUserAuthorizedAdaccounts",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-user-id&#125;/authorized_adaccounts?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram User Authorized Adaccounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85bb7af7-8f01-4f45-9408-a8473db864ae"
            }
          ]
        },
        {
          "id": "3b2ef76d-54f3-475a-84fb-d5acc8422c6e",
          "name": "getInstagramMedia",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-media-id&#125;?caption_textstring=caption_textstring&comment_countint32=comment_countint32&content_typeint32=content_typeint32&display_urlstring=display_urlstring&filter_namestring=filter_namestring&idnumeric string=idnumeric%20string&latitudefloat=latitudefloat&like_countint32=like_countint32&locationLocation=locationLocation&location_namestring=location_namestring&longitudefloat=longitudefloat&owner_instagram_userInstagramUser=owner_instagram_userInstagramUser&permalinkstring=permalinkstring&taken_atdatetime=taken_atdatetime&video_urlstring=video_urlstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c285694-2799-4557-962c-2ca9ca583e83"
            }
          ]
        },
        {
          "id": "d04f9efc-5c6d-426f-ba78-4d2327e5af02",
          "name": "getInstagramComment",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-comment-id&#125;?comment_typeenum=comment_typeenum&created_atdatetime=created_atdatetime&idstring=idstring&instagram_comment_idnumeric string=instagram_comment_idnumeric%20string&instagram_userInstagramUser=instagram_userInstagramUser&mentioned_instagram_userslistInstagramUser=mentioned_instagram_userslistInstagramUser&messagestring=messagestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram Comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f528c575-8b92-4bdd-b782-60bc74b7f48c"
            }
          ]
        },
        {
          "id": "1cecb24b-0905-4f9a-8f1f-6effa620db0c",
          "name": "getInstagramCarousel",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-carousel-id&#125;?caption_textstring=caption_textstring&comment_countint32=comment_countint32&content_typeint32=content_typeint32&display_urlstring=display_urlstring&idnumeric string=idnumeric%20string&like_countint32=like_countint32&owner_instagram_userInstagramUser=owner_instagram_userInstagramUser&permalinkstring=permalinkstring&taken_atdatetime=taken_atdatetime&video_urlstring=video_urlstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram Carousel"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea73769e-da1f-4080-900c-4c22e571ec50"
            }
          ]
        }
      ]
    }
  ]
}