---
swagger: "2.0"
x-collection-name: Gmail
x-complete: 0
info:
  title: Gmail Get History
  description: Lists the history of all changes to the given mailbox. History results
    are returned in chronological order (increasing historyId).
  contact:
    name: Google
    url: https://google.com
  version: v1
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