swagger: "2.0"
x-collection-name: PayRun
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
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
  /Jobs/Rti/{JobId}/Status:
    get:
      summary: Get the RTI job status
      description: Return the the RTI job status
      operationId: GetRtiJobStatus
      x-api-path-slug: jobsrtijobidstatus-get
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
      - Status
  /Reports:
    get:
      summary: Gets all reports
      description: Get links to all saved report definitions under authorised application
      operationId: GetReportDefinitionsFromApplication
      x-api-path-slug: reports-get
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
      - Reports
  /Schemas:
    get:
      summary: Get a list of all available schemas
      description: Returns a collection of links to all the available data object
        schemas
      operationId: GetSchemas
      x-api-path-slug: schemas-get
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
      - List
      - Of
      - ""
      - Available
      - Schemas
  /Employer/{EmployerId}/Employees/Tag/{TagId}:
    get:
      summary: Get employees with tag
      description: Gets the employees with the tag
      operationId: GetEmployeesWithTag
      x-api-path-slug: employeremployeridemployeestagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - Tag