---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Veo Comments
  description: All of the comments on this video.
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{video}/likes:
    get:
      summary: Get Veo Likes
      description: Users who like this video.
      operationId: getVeoLikes
      x-api-path-slug: videolikes-get
      parameters:
      - in: path
        name: video
        description: Represents the ID of the video object
      responses:
        200:
          description: OK
      tags:
      - Video
      - Likes
  /{video}/comments:
    get:
      summary: Get Veo Comments
      description: All of the comments on this video.
      operationId: getVeoComments
      x-api-path-slug: videocomments-get
      parameters:
      - in: path
        name: video
        description: Represents the ID of the video object
      responses:
        200:
          description: OK
      tags:
      - Video
      - Comments
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