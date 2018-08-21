---
swagger: "2.0"
x-collection-name: Swagger
x-complete: 0
info:
  title: Swagger Hub Registry Gets API's collaboration
  description: Gets api's collaboration.
  contact:
    name: SwaggerHub
    url: http://swaggerhub.com
    email: info@swaggerhub.com
  version: 1.0.45
host: api.swaggerhub.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apis:
    get:
      summary: Retrieves a list of currently defined APIs in APIs.json format.
      description: Retrieves a list of currently defined apis in apis.json format..
      operationId: searchApis
      x-api-path-slug: apis-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: order
        description: sort order
      - in: query
        name: page
        description: page to return
      - in: query
        name: query
        description: free text query to match
      - in: query
        name: sort
        description: sort criteria or result set* NAME -* UPATED* CREATED* OWNER
      - in: query
        name: state
        description: matches against published state of the spec* UNPUBLISHED - spec
          is a draft, a work in progress* PUBLISHED - spec is a stable version ready
          for consuming from client applications* ANY - either PUBLISHED or UNPUBLISHED
      - in: query
        name: tag
        description: matches against tags associated with an API
      responses:
        200:
          description: OK
      tags:
      - APIs
  /specs:
    get:
      summary: Retrieves a list of currently defined APIs and Domains in APIs.json
        format
      description: Retrieves a list of currently defined apis and domains in apis.json
        format.
      operationId: searchApisAndDomains
      x-api-path-slug: specs-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: order
        description: sort order
      - in: query
        name: owner
        description: API or Domaion owner identifier
      - in: query
        name: page
        description: page to return
      - in: query
        name: query
        description: free text query to match
      - in: query
        name: sort
        description: sort criteria or result set* NAME -* UPATED* CREATED* OWNER
      - in: query
        name: specType
        description: Type of Swagger specs to search* API - APIs only* DOMAIN - Domains
          only* ANY - Both APIs and Domains
      - in: query
        name: state
        description: matches against published state of the spec* UNPUBLISHED - spec
          is a draft, a work in progress* PUBLISHED - spec is a stable version ready
          for consuming from client applications* ANY - either PUBLISHED or UNPUBLISHED
      - in: query
        name: visibility
        description: The visibility of a spec in SwaggerHub* PUBLIC - can be viewed
          by anyone* PRIVATE - can only be viewed by you or your Org and those that
          you are collaborating with or have shared it with* ANY - either PUBLIC or
          PRIVATE
      responses:
        200:
          description: OK
      tags:
      - Specs
  /domains:
    get:
      summary: Retrieves a list of currently defined domains in APIs.json format
      description: Retrieves a list of currently defined domains in apis.json format.
      operationId: searchDomains
      x-api-path-slug: domains-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: order
        description: sort order
      - in: query
        name: page
        description: page to return
      - in: query
        name: query
        description: free text query to match
      - in: query
        name: sort
        description: sort criteria or result set* NAME -* UPATED* CREATED* OWNER
      - in: query
        name: state
        description: matches against published state of the spec* UNPUBLISHED - spec
          is a draft, a work in progress* PUBLISHED - spec is a stable version ready
          for consuming from client applications* ANY - either PUBLISHED or UNPUBLISHED
      - in: query
        name: tag
        description: matches against tags associated with a domain
      responses:
        200:
          description: OK
      tags:
      - Domains
  /apis/{owner}/{api}/.collaboration:
    get:
      summary: Gets API's collaboration
      description: Gets api's collaboration.
      operationId: getCollaboration
      x-api-path-slug: apisownerapi-collaboration-get
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: query
        name: expandTeams
      - in: path
        name: owner
        description: API or Domaion owner identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - ""
      - Collaboration
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