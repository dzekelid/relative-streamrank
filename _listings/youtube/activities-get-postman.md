{
  "info": {
    "name": "YouTube",
    "_postman_id": "3541e12e-3337-4190-86bf-f2bcda550389",
    "description": "YouTube allows users to upload, view, rate, share, add to favorites, report, comment on videos, and subscribe to other users. It offers a wide variety of user-generated and corporate media videos. Available content includes video clips, TV show clips, music videos, short and documentary films, audio recordings, movie trailers, live streams, and other content such as video blogging, short original videos, and educational videos. Most of the content on YouTube is uploaded by individuals, but media corporations including CBS, the BBC, Vevo, and Hulu offer some of their material via YouTube as part of the YouTube partnership program. Unregistered users can only watch videos on the site, while registered users are permitted to upload an unlimited number of videos and add comments to videos.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "activities",
      "item": [
        {
          "id": "66f8089e-9fe0-495a-8f1e-91dd9bcc75c5",
          "name": "getActivities",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/activities?channelId=%7B%7D&home=%7B%7D&maxResults=%7B%7D&mine=%7B%7D&pageToken=%7B%7D&part=%7B%7D&publishedAfter=%7B%7D&publishedBefore=%7B%7D&regionCode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of channel activity events that match the request criteria"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81a4c188-0165-4ef6-85f2-c95532f8f283"
            }
          ]
        }
      ]
    }
  ]
}