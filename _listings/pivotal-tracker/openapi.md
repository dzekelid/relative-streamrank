---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 1
info:
  title: Pivotal Tracker
  description: access-and-manipulate-agile-project-management-data-including-projects-stories-and-tasks-
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
  /projects/{PROJECT_ID}/iterations/done:
    get:
      summary: Get Projects Project Iterations Done
      description: Retrieves iterations from the "done" group, with stories.
      operationId: getProjectsProjectIterationsDone
      x-api-path-slug: projectsproject-iditerationsdone-get
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
      - Done
  /projects/{PROJECT_ID}/memberships:
    get:
      summary: Get Projects Project Memberships
      description: Retrieves all memberships for a project.
      operationId: getProjectsProjectMemberships
      x-api-path-slug: projectsproject-idmemberships-get
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
      - Memberships
  /projects/{PROJECT_ID}/stories:
    get:
      summary: Get Projects Project Stories
      description: Retrieves all stories for a project, or those matching filter(s)
      operationId: getProjectsProjectStories
      x-api-path-slug: projectsproject-idstories-get
      parameters:
      - in: query
        name: filter
        description: A filter for the returned stories to match
      - in: query
        name: limit
        description: Controls the maximum number of stories returned
      - in: query
        name: offset
        description: Controls the number of stories to skip from the beginning of
          the result
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
      - Stories
  /projects/{PROJECT_ID}/stories/{STORY_ID}/tasks:
    get:
      summary: Get Projects Project Stories Story Tasks
      description: Get projects project stories story tasks.
      operationId: getProjectsProjectStoriesStoryTasks
      x-api-path-slug: projectsproject-idstoriesstory-idtasks-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
---