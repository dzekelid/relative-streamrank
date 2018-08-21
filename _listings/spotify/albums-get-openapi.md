---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 0
info:
  title: Spotify Get Albums
  description: '[Get Several Albums](https://developer.spotify.com/web-api/get-several-albums/)'
  version: v1
host: api.spotify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /albums:
    get:
      summary: Get Albums
      description: '[Get Several Albums](https://developer.spotify.com/web-api/get-several-albums/)'
      operationId: get-several-albumshttpsdeveloperspotifycomwebapigetseveralalbums
      x-api-path-slug: albums-get
      parameters:
      - in: query
        name: ids
        description: A comma-separated list of IDs
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      responses:
        200:
          description: OK
      tags:
      - Music
      - Albums
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---