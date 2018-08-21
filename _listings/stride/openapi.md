---
swagger: "2.0"
x-collection-name: Stride
x-complete: 1
info:
  title: Stride
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
host: api.atlassian.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation:
    get:
      summary: Get conversation list for site
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationByCloudIdGet
      x-api-path-slug: sitecloudidconversation-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: query
        name: cursor
      - in: query
        name: include-archived
      - in: query
        name: include-private
      - in: query
        name: limit
      - in: query
        name: query
      - in: query
        name: sort
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
  /site/{cloudId}/conversation/{conversationId}:
    get:
      summary: Get conversation details
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
  /site/{cloudId}/conversation/{conversationId}/roster:
    get:
      summary: Get conversation roster
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationRosterByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidroster-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: query
        name: limit
      - in: query
        name: start
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Roster
---