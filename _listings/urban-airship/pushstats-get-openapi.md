---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Get Push Stats
  description: 'Returns hourly message counts for your application. By default, results
    are returned in JSON. For CSV, either add the header:Accept:text/csv or append
    &format=csv to the query string. Times are in UTC, and data is provided for each
    push platform (currently: iOS, BlackBerry, Android, and C2DM, in that order).
    The statistics system is updated every 15 minutes, so the final count for an hour
    will be done at the latest 15 minutes after the hour is done.'
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /feeds:
    get:
      summary: Get Feeds
      description: Gets a list of feeds.
      operationId: feeds.get
      x-api-path-slug: feeds-get
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Feeds
  /partner/apps:
    get:
      summary: Get Partner Apps
      description: List applications.
      operationId: partner.apps.get
      x-api-path-slug: partnerapps-get
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      responses:
        200:
          description: OK
      tags:
      - Partner
      - Apps
  /push/stats:
    get:
      summary: Get Push Stats
      description: 'Returns hourly message counts for your application. By default,
        results are returned in JSON. For CSV, either add the header:Accept:text/csv
        or append &format=csv to the query string. Times are in UTC, and data is provided
        for each push platform (currently: iOS, BlackBerry, Android, and C2DM, in
        that order). The statistics system is updated every 15 minutes, so the final
        count for an hour will be done at the latest 15 minutes after the hour is
        done.'
      operationId: push.stats.get
      x-api-path-slug: pushstats-get
      parameters:
      - in: query
        name: end
        description: End date in UTC format
      - in: query
        name: format
        description: Response format
      - in: query
        name: start
        description: Start date in UTC format
      responses:
        200:
          description: OK
      tags:
      - Push
      - Stats
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