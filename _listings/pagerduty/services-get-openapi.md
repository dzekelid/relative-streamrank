---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty List services
  version: 1.0.0
  description: List existing services.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notifications:
    get:
      summary: List notifications
      description: List notifications for a given time range, optionally filtered
        by type (sms_notification, email_notification, phone_notification, or push_notification).
      operationId: list-notifications-for-a-given-time-range-optionally-filtered-by-type-sms-notification-email-notific
      x-api-path-slug: notifications-get
      parameters:
      - in: query
        name: filter
        description: Return notification of this type only
      - in: query
        name: include[]
        description: Array of additional details to include
      - in: query
        name: No Name
      - in: query
        name: since
        description: The start of the date range over which you want to search
      - in: query
        name: until
        description: The end of the date range over which you want to search
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /services:
    get:
      summary: List services
      description: List existing services.
      operationId: list-existing-services
      x-api-path-slug: services-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional details to include
      - in: query
        name: No Name
      - in: query
        name: query
        description: Filters the result, showing only the services whose name or service_key
          matches the query
      responses:
        200:
          description: OK
      tags:
      - Services
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