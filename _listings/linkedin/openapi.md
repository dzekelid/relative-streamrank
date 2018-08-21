---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 1
info:
  title: LinkedIn
  description: bring-user-profiles-and-professional-networks-to-your-apps-
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/:
    get:
      summary: Get Companies
      description: Get companies
      operationId: getCompanies
      x-api-path-slug: companies-get
      responses:
        200:
          description: OK
      tags:
      - Companies
  /people/~:
    get:
      summary: Get People
      description: Get people ~
      operationId: getPeople~
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - People
  /companies/{id}/updates:
    get:
      summary: Get Companies Updates
      description: Get companies  updates
      operationId: getCompaniesUpdates
      x-api-path-slug: companiesidupdates-get
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Updates
---