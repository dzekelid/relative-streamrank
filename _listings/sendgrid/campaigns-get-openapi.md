---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Campaigns
  description: |-
    **This endpoint allows you to retrieve a list of all of your campaigns.**

    Returns campaigns in reverse order they were created (newest first).

    Returns an empty array if no campaigns exist.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/stats:
    get:
      summary: Get Devices Stats
      description: "**This endpoint allows you to retrieve your email statistics segmented
        by the device type.**\n\n**We only store up to 7 days of email activity in
        our database.** By default, 500 items will be returned per request via the
        Advanced Stats API endpoints.\n\n## Available Device Types\n| **Device** |
        **Description** | **Example** |\n|---|---|---|\n| Desktop | Email software
        on desktop computer. | I.E., Outlook, Sparrow, or Apple Mail. |\n| Webmail
        |\tA web-based email client. | I.E., Yahoo, Google, AOL, or Outlook.com. |\n|
        Phone | A smart phone. | iPhone, Android, Blackberry, etc.\n| Tablet | A tablet
        computer. | iPad, android based tablet, etc. |\n| Other | An unrecognized
        device. |\n\nAdvanced Stats provide a more in-depth view of your email statistics
        and the actions taken by your recipients. You can segment these statistics
        by geographic location, device type, client type, browser, and mailbox provider.
        For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html)."
      operationId: devices.stats.get
      x-api-path-slug: devicesstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: How many results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: How many results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Devices
      - Stats
  /categories/stats:
    get:
      summary: Get Categories Stats
      description: |-
        **This endpoint allows you to retrieve all of your email statistics for each of your categories.**

        If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

        Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
      operationId: categories.stats.get
      x-api-path-slug: categoriesstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: categories
        description: The individual categories that you want to retrieve statistics
          for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to skip
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
      - Stats
  /campaigns:
    get:
      summary: Get Campaigns
      description: |-
        **This endpoint allows you to retrieve a list of all of your campaigns.**

        Returns campaigns in reverse order they were created (newest first).

        Returns an empty array if no campaigns exist.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: GET_campaigns
      x-api-path-slug: campaigns-get
      parameters:
      - in: query
        name: limit
        description: The number of results you would like to receive at a time
      - in: query
        name: offset
        description: The index of the first campaign to return, where 0 is the first
          campaign
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
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