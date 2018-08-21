---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Devices Stats
  description: "**This endpoint allows you to retrieve your email statistics segmented
    by the device type.**\n\n**We only store up to 7 days of email activity in our
    database.** By default, 500 items will be returned per request via the Advanced
    Stats API endpoints.\n\n## Available Device Types\n| **Device** | **Description**
    | **Example** |\n|---|---|---|\n| Desktop | Email software on desktop computer.
    | I.E., Outlook, Sparrow, or Apple Mail. |\n| Webmail |\tA web-based email client.
    | I.E., Yahoo, Google, AOL, or Outlook.com. |\n| Phone | A smart phone. | iPhone,
    Android, Blackberry, etc.\n| Tablet | A tablet computer. | iPad, android based
    tablet, etc. |\n| Other | An unrecognized device. |\n\nAdvanced Stats provide
    a more in-depth view of your email statistics and the actions taken by your recipients.
    You can segment these statistics by geographic location, device type, client type,
    browser, and mailbox provider. For more information about statistics, please see
    our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html)."
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