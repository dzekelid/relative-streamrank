---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 0
info:
  title: Pivotal Tracker Get Projects Project Iterations Current Backlog
  description: Retrieves iterations from the "current" and "backlog" groups, with
    stories.
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities:
    get:
      summary: Get Activities
      description: Retrieves the recent activity of all your projects.
      operationId: getActivities
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of activity feed items
      - in: query
        name: newer_than_version
        description: Restricts the activity feed to only those items that have a greater
          than supplied version
      - in: query
        name: occurred_since_date
        description: 'Restricts the activity feed to only those items that occurred
          after a supplied date (example format: 2009/12/18 21:00:00 UTC)'
      responses:
        200:
          description: OK
      tags:
      - Activities
  /projects:
    get:
      summary: Get Projects
      description: Retrieves all of the user's projects.
      operationId: getProjects
      x-api-path-slug: projects-get
      responses:
        200:
          description: OK
      tags:
      - Projects
  /projects/{PROJECT_ID}/iterations:
    get:
      summary: Get Projects Project Iterations
      description: Retrieves all iterations, with stories.
      operationId: getProjectsProjectIterations
      x-api-path-slug: projectsproject-iditerations-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
  /projects/{PROJECT_ID}/iterations/current:
    get:
      summary: Get Projects Project Iterations Current
      description: Retrieves iterations from the "current" group, with stories.
      operationId: getProjectsProjectIterationsCurrent
      x-api-path-slug: projectsproject-iditerationscurrent-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
      - Current
  /projects/{PROJECT_ID}/iterations/current_backlog:
    get:
      summary: Get Projects Project Iterations Current Backlog
      description: Retrieves iterations from the "current" and "backlog" groups, with
        stories.
      operationId: getProjectsProjectIterationsCurrentBacklog
      x-api-path-slug: projectsproject-iditerationscurrent-backlog-get
      parameters:
      - in: query
        name: limit
        description: Controls the maximum number of iterations returned
      - in: query
        name: offset
        description: Controls the number of iterations to skip from the beginning
          of the result
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
      - Current
      - Backlog
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