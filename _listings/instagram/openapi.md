swagger: "2.0"
x-collection-name: Instagram
x-complete: 1
info:
  title: Instagram
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;instagram-carousel-id&#125;:
    get:
      summary: Instagram Carousel
      description: Instagram Carousel
      operationId: getInstagramCarousel
      x-api-path-slug: 123instagramcarouselid125-get
      parameters:
      - in: query
        name: caption_textstring
        description: Caption text
        type: string
      - in: query
        name: comment_countint32
        description: Number of comments
        type: string
      - in: query
        name: content_typeint32
        description: 0 for photo, 1 for video
        type: string
      - in: query
        name: display_urlstring
        description: URL of the photo or cover frame
        type: string
      - in: query
        name: idnumeric string
        description: ID of the Instagram carousel
        type: string
      - in: query
        name: like_countint32
        description: Number of likes
        type: string
      - in: query
        name: owner_instagram_userInstagramUser
        description: The Instagram user that owns this carousel
        type: string
      - in: query
        name: permalinkstring
        description: Instagram permalink of the first asset
        type: string
      - in: query
        name: taken_atdatetime
        description: When the media was created
        type: string
      - in: query
        name: video_urlstring
        description: URL of the video
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Carousel
  /&#123;instagram-carousel-id&#125;/comments:
    get:
      summary: Instagram Carousel Comments
      description: Instagram Carousel Comments
      operationId: getInstagramCarouselComments
      x-api-path-slug: 123instagramcarouselid125comments-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Carousel
      - Comments
  /&#123;instagram-media-id&#125;/comments:
    get:
      summary: Instagram Media Comments
      description: Instagram Media Comments
      operationId: getInstagramMediaComments
      x-api-path-slug: 123instagrammediaid125comments-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Media
      - Comments
  /&#123;instagram-user-id&#125;:
    get:
      summary: Instagram User
      description: Instagram User
      operationId: getInstagramUser
      x-api-path-slug: 123instagramuserid125-get
      parameters:
      - in: query
        name: followed_by_countint32
        description: Number of Instagram users that follow this Instagram user
        type: string
      - in: query
        name: follow_countint32
        description: Number of Instagram users that this Instagram user follows
        type: string
      - in: query
        name: has_profile_picturebool
        description: Indicates whether Instagram Account has a profile picture
        type: string
      - in: query
        name: idnumeric string
        description: ID of the Instagram user
        type: string
      - in: query
        name: is_privatebool
        description: Whether the Instagram user is private
        type: string
      - in: query
        name: is_publishedbool
        description: Whether the Instagram user is published
        type: string
      - in: query
        name: media_countint32
        description: Number of active media posted by this Instagram user
        type: string
      - in: query
        name: profile_picstring
        description: URI to user&#039;s Instagram profile picture
        type: string
      - in: query
        name: usernamestring
        description: Instagram username
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - User