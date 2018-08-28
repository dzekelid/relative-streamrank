swagger: "2.0"
x-collection-name: SugarSync
x-complete: 1
info:
  title: SugarSync  API
  description: the-sugarsync-service-presents-a-set-of-resources-that-your-application-can-access-through-the-platform-api--
  version: "1"
host: api.sugarsync.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /folder:
    get:
      summary: Retrieving Folder Information
      description: To retrieve information about a folder, an application submits
        an HTTP GET request to then          folder resource that represents the folder.
      operationId: retrieving-folder-information
      x-api-path-slug: folder-get
      responses:
        200:
          description: OK
      tags:
      - Folder
  /receivedShare/:
    get:
      summary: Retrieving Received Share Information
      description: To retrieve information about a received share (that is, a shared
        folder owned by another user and to whichnthis user has been granted access
        privileges by the owner), an application submits an HTTP GET request to the
        URLnthat represents the received share resource. The URL is referenced in
        the &lt;receivedShare&gt; element for the received share in the received shares
        list.nSee Retrieving the Received Shares List.
      operationId: retrieving-received-share-information
      x-api-path-slug: receivedshare-get
      responses:
        200:
          description: OK
      tags:
      - ReceivedShare
  /workspace:
    get:
      summary: Retrieving Workspace Information
      description: To retrieve information about a workspace, an application submits
        an HTTP GET request to then          workspace resource that represents the
        workspace.
      operationId: retrieving-workspace-information
      x-api-path-slug: workspace-get
      responses:
        200:
          description: OK
      tags:
      - Workspace
  /file:
    get:
      summary: Retrieving File Data
      description: To retrieve file data, an application submits an HTTP GET request
        to then          file data resource that represents the data for the file.
      operationId: retrieving-file-data
      x-api-path-slug: file-get
      responses:
        200:
          description: OK
      tags:
      - File
  /album/:
    get:
      summary: Retrieving Album Information
      description: To retrieve information about an album, an application submits
        an HTTP GET request to then          album resource that represents the album.
      operationId: retrieving-album-information
      x-api-path-slug: album-get
      parameters:
      - in: query
        name: max
        description: Positive integer
      - in: query
        name: order
        description: name, last_modified, size, or extension
      - in: query
        name: start
        description: 0 or positive integer
      responses:
        200:
          description: OK
      tags:
      - Album