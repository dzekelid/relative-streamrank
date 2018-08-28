swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
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
  /user/{user_id}/messages:
    get:
      summary: Get User User Messages
      description: Returns a list of messages and some metadata about them. It will
        also include some metadata about the user.
      operationId: user.user_id.messages.get
      x-api-path-slug: useruser-idmessages-get
      parameters:
      - in: query
        name: full_list
        description: Get the full message included in this list (which might take
          a while to download)
      - in: query
        name: since
        description: Return only new items
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages