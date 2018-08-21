---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 0
info:
  title: OpenDataSoft Get Source Datasets
  description: |-
    List of available datasets, each with their endpoints, paginated.

    Links provided:
    * previous page
    * next page
    * last page
    * first page
  version: 2.1.0
host: public.opendatasoft.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pages:
    get:
      summary: Get Pages
      description: List of all pages from this portal.
      operationId: getPages
      x-api-path-slug: pages-get
      responses:
        200:
          description: OK
      tags:
      - Pages
  /{source}/datasets:
    get:
      summary: Get Source Datasets
      description: |-
        List of available datasets, each with their endpoints, paginated.

        Links provided:
        * previous page
        * next page
        * last page
        * first page
      operationId: getDatasets
      x-api-path-slug: sourcedatasets-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
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