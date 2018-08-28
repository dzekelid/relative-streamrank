swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
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
  /tasks:
    post:
      summary: Create Task
      description: Used to create a single task for single user on a single file.
      operationId: createTask
      x-api-path-slug: tasks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Tasks
  /files/{FILE_ID}/collaborations:
    get:
      summary: Get File's Collaborations
      description: Use this to get a list of all the collaborations on a file
      operationId: getFileCollaborations
      x-api-path-slug: filesfile-idcollaborations-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FILE_ID
      - in: query
        name: limit
        description: The maximum number of items to return in a page
      - in: query
        name: offset
        description: The item at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Collaborations