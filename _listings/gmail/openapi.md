swagger: "2.0"
x-collection-name: Gmail
x-complete: 1
info:
  title: Gmail
  version: 1.0.0
host: www.googleapis.com
basePath: /gmail/v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{userId}/history:
    get:
      summary: Get History
      description: Lists the history of all changes to the given mailbox. History
        results are returned in chronological order (increasing historyId).
      operationId: gmail.users.history.list
      x-api-path-slug: useridhistory-get
      parameters:
      - in: query
        name: historyTypes
        description: History types to be returned by the function
      - in: query
        name: labelId
        description: Only return messages with a label matching the ID
      - in: query
        name: maxResults
        description: The maximum number of history records to return
      - in: query
        name: pageToken
        description: Page token to retrieve a specific page of results in the list
      - in: query
        name: startHistoryId
        description: Required
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - History
  /{userId}/watch:
    post:
      summary: Send Push Notification
      description: Set up or update a push notification watch on the given user mailbox.
      operationId: gmail.users.watch
      x-api-path-slug: useridwatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: The users email address
      responses:
        200:
          description: OK
      tags:
      - Push Notification