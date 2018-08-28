swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{video}/likes:
    get:
      summary: Get Veo Likes
      description: Users who like this video.
      operationId: getVeoLikes
      x-api-path-slug: videolikes-get
      parameters:
      - in: path
        name: video
        description: Represents the ID of the video object
      responses:
        200:
          description: OK
      tags:
      - Video
      - Likes
  /{video}/comments:
    get:
      summary: Get Veo Comments
      description: All of the comments on this video.
      operationId: getVeoComments
      x-api-path-slug: videocomments-get
      parameters:
      - in: path
        name: video
        description: Represents the ID of the video object
      responses:
        200:
          description: OK
      tags:
      - Video
      - Comments
  /{user}/videos:
    get:
      summary: Get User Veos
      description: The videos this user has been tagged in
      operationId: getUserVeos
      x-api-path-slug: uservideos-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Videos
  /{user}/statuses:
    get:
      summary: Get User Statuses
      description: The user's status updates
      operationId: getUserStatuses
      x-api-path-slug: userstatuses-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Statuses
  /{user}/posts:
    get:
      summary: Get User Adds
      description: The user's posts
      operationId: getUserAdds
      x-api-path-slug: userposts-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Posts
  /{user}/photos:
    get:
      summary: Get User Photos
      description: The photos the user is tagged in
      operationId: getUserPhotos
      x-api-path-slug: userphotos-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Photos
  /{user}/likes:
    get:
      summary: Get User Likes
      description: All the pages this user has liked.
      operationId: getUserLikes
      x-api-path-slug: userlikes-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Likes
  /{user}/friends:
    get:
      summary: Get User Friends
      description: The user's friends
      operationId: getUserFriends
      x-api-path-slug: userfriends-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Friends
  /{user}/events:
    get:
      summary: Get User Events
      description: The events this user is attending.
      operationId: getUserEvents
      x-api-path-slug: userevents-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Events