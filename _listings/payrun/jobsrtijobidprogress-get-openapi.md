---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Get the RTI job progress
  description: Return the the RTI job progress
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employers:
    get:
      summary: Gets all employers
      description: Gets links to all employers contained under the authorised application
        scope
      operationId: GetEmployers
      x-api-path-slug: employers-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ""
      - Employers
  /Healthcheck:
    get:
      summary: Get health check status
      description: Returns the health status of the application
      operationId: GetHealthCheck
      x-api-path-slug: healthcheck-get
      responses:
        200:
          description: OK
      tags:
      - Health
      - Check
      - Status
  /Jobs/PayRuns:
    get:
      summary: Get all PayRun jobs
      description: Gets all the pay run jobs
      operationId: GetPayRunJobs
      x-api-path-slug: jobspayruns-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PayRun
      - Jobs
  /Jobs/Dps/{JobId}/Progress:
    get:
      summary: Get the DPS job progress
      description: Return the the DPS job progress
      operationId: GetDpsJobProgress
      x-api-path-slug: jobsdpsjobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPJob
      - Progress
  /Query:
    post:
      summary: Get the query result
      description: Get the results for the specified query
      operationId: GetQueryResponse
      x-api-path-slug: query-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Query
        description: The query object to be executed against the application data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Query
      - Result
  /Jobs/Rti/{JobId}/Progress:
    get:
      summary: Get the RTI job progress
      description: Return the the RTI job progress
      operationId: GetRtiJobProgress
      x-api-path-slug: jobsrtijobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Progress
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