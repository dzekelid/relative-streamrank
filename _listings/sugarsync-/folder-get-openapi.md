---
swagger: "2.0"
x-collection-name: SugarSync
x-complete: 0
info:
  title: Sugar Sync  API Retrieving Folder Information
  description: To retrieve information about a folder, an application submits an HTTP
    GET request to then          folder resource that represents the folder.
  version: "1"
host: api.sugarsync.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /folder:
    get:
      summary: Retrieving Folder Information
      description: To retrieve information about a folder, an application submits
        an HTTP GET request to then          folder resource that represents the folder.
      operationId: retrieving-folder-information
      x-api-path-slug: folder-get
      responses:
        200:
          description: OK
      tags:
      - Folder
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