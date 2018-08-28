swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/search/{query}:
    get:
      summary: Search Users
      description: This API allows to find users.
      operationId: getUsersSearchQuery
      x-api-path-slug: userssearchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Users
  /episodes/live:
    get:
      summary: Get Live Episodes
      description: Retrieves all live episodes at the moment of the request
      operationId: getEpisodesLive
      x-api-path-slug: episodeslive-get
      parameters:
      - in: query
        name: show_id
        description: An list of show_id applied as a filter
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Live
      - Episodes
  /show/search/{query}:
    get:
      summary: Search Shows
      description: This API allows to find shows.
      operationId: getShowSearchQuery
      x-api-path-slug: showsearchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Shows
  /user/{user_id}/actions:
    get:
      summary: Get User Actions
      description: Retrieves the user actions settings
      operationId: getUserUserActions
      x-api-path-slug: useruser-idactions-get
      parameters:
      - in: query
        name: EPISODE_BROADCAST
        description: The user has published a new episode ( either live or podcast
          )
      - in: query
        name: FACEBOOK
        description: The user wants to share on facebook the specified action
      - in: query
        name: RADIO_FOLLOW
        description: The user starts following a radio
      - in: query
        name: RADIO_MESSAGE
        description: The user has sent a message to a radio
      - in: query
        name: SHOW_FOLLOW
        description: The user starts following a show
      - in: query
        name: SHOW_MESSAGE
        description: The user has sent a message to a show
      - in: query
        name: TWITTER
        description: The user wants to share on twitter the specified action
      - in: query
        name: USER_FOLLOW
        description: The user starts following another user
      - in: query
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - User
      - Actions