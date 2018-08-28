swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 1
info:
  title: PagerDuty
  version: 1.0.0
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
  /incidents:
    get:
      summary: List incidents
      description: List existing incidents.
      operationId: list-existing-incidents
      x-api-path-slug: incidents-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional details to include
      - in: query
        name: No Name
      - in: query
        name: sort_by
        description: Used to specify both the field you wish to sort the results on
          (incident_number/created_on/resolved_on/urgency), as well as the direction
          (asc/desc) of the results
      - in: query
        name: statuses[]
        description: Return only incidents with the given statuses
      responses:
        200:
          description: OK
      tags:
      - Incidents
  /log_entries:
    get:
      summary: List log entries
      description: List all of the incident log entries across the entire account.
      operationId: list-all-of-the-incident-log-entries-across-the-entire-account
      x-api-path-slug: log-entries-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Log Entries