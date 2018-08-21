---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box User Events, Enterprise Events
  description: |-
    Use this to get events for a given user. A chunk of event objects is returned for the user based on the parameters passed in. Parameters indicating how many chunks are left as well as the next stream_position are also returned.

    To retrieve Enterprise Events specify 'stream_type=admin_logs'. Retrieves up to a year' events for all users in an enterprise. Upper and lower bounds as well as filters can be applied to the results.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborations:
    get:
      summary: Pending Collaborations
      description: Used to retrieve all pending collaboration invites for this user.
      operationId: getPendingCollaborations
      x-api-path-slug: collaborations-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: query
        name: status
        description: Must be pending
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Collaborations
  /events:
    get:
      summary: User Events, Enterprise Events
      description: |-
        Use this to get events for a given user. A chunk of event objects is returned for the user based on the parameters passed in. Parameters indicating how many chunks are left as well as the next stream_position are also returned.

        To retrieve Enterprise Events specify 'stream_type=admin_logs'. Retrieves up to a year' events for all users in an enterprise. Upper and lower bounds as well as filters can be applied to the results.
      operationId: getUserEvents
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: created_after
        description: A lower bound on the timestamp of the events returned
      - in: query
        name: created_before
        description: An upper bound on the timestamp of the events returned
      - in: query
        name: event_type
        description: A comma-separated list of events to filter by
      - in: query
        name: limit
        description: Limits the number of events returned
      - in: query
        name: stream_position
        description: The location in the event stream at which you want to start receiving
          events
      - in: query
        name: stream_type
        description: 'Limits the type of events returned: all: returns everything,
          changes: returns tree changes, sync: returns tree changes only for sync
          folders'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Events
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