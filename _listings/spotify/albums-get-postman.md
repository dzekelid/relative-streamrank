{
  "info": {
    "name": "Spotify",
    "_postman_id": "5e186494-e428-4711-a300-b25dc6e37d9e",
    "description": "Our Web API lets your applications fetch data from the Spotify music catalog and manage user&rsquo;s playlists and saved music. Based on simple REST principles, our Web API endpoints return metadata in JSON format about artists, albums, and tracks directly from the Spotify catalogue. The API also provides access to user-related data such as playlists and music saved in a &ldquo;Your Music&rdquo; library, subject to user&rsquo;s authorization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "0ef4f9a3-d5cb-4e0e-b4d2-eea33bff16e0",
          "name": "get-several-albumshttpsdeveloperspotifycomwebapigetseveralalbums",
          "request": {
            "url": "http://api.spotify.com/v1/albums?ids=%7B%7D&market=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "[Get Several Albums](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf427e82-0969-4ff2-b8e9-7512b66e8af5"
            }
          ]
        }
      ]
    }
  ]
}