---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Get Subscriptions
  description: Returns subscription resources that match the API request criteria.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /liveBroadcasts:
    get:
      summary: Get Live Broadcasts
      description: Returns a list of YouTube broadcasts that match the API request
        parameters.
      operationId: getLivebroadcasts
      x-api-path-slug: livebroadcasts-get
      parameters:
      - in: query
        name: broadcastStatus
        description: The broadcastStatus parameter filters the API response to only
          include broadcasts with the specified status
      - in: query
        name: broadcastType
        description: The broadcastType parameter filters the API response to only
          include broadcasts with the specified type
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of YouTube
          broadcast IDs that identify the broadcasts being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: The mine parameter can be used to instruct the API to only return
          broadcasts owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
  /liveChat/messages:
    get:
      summary: Get Live Chat Messages
      description: Lists live chat messages for a specific chat.
      operationId: getLivechatMessages
      x-api-path-slug: livechatmessages-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter instructs the API to retrieve localized resource
          metadata for a specific application language that the YouTube website supports
      - in: query
        name: liveChatId
        description: The liveChatId parameter specifies the ID of the chat whose messages
          will be returned
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of messages
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies the liveChatComment resource parts
          that the API response will include
      - in: query
        name: profileImageSize
        description: The profileImageSize parameter specifies the size of the user
          profile pictures that should be returned in the result set
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Messages
  /liveStreams:
    get:
      summary: Get Livestreams
      description: Returns a list of video streams that match the API request parameters.
      operationId: getLivestreams
      x-api-path-slug: livestreams-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of YouTube
          stream IDs that identify the streams being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: The mine parameter can be used to instruct the API to only return
          streams owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveStream resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Livestreams
  /reports:
    get:
      summary: Get Reports
      description: Retrieve your YouTube Analytics reports.
      operationId: getReports
      x-api-path-slug: reports-get
      parameters:
      - in: query
        name: currency
        description: The currency to which financial metrics should be converted
      - in: query
        name: dimensions
        description: A comma-separated list of YouTube Analytics dimensions, such
          as views or ageGroup,gender
      - in: query
        name: end-date
        description: The end date for fetching YouTube Analytics data
      - in: query
        name: filters
        description: A list of filters that should be applied when retrieving YouTube
          Analytics data
      - in: query
        name: ids
        description: Identifies the YouTube channel or content owner for which you
          are retrieving YouTube Analytics data
      - in: query
        name: include-historical-channel-data
        description: If set to true historical data (i
      - in: query
        name: max-results
        description: The maximum number of rows to include in the response
      - in: query
        name: metrics
        description: A comma-separated list of YouTube Analytics metrics, such as
          views or likes,dislikes
      - in: query
        name: sort
        description: A comma-separated list of dimensions or metrics that determine
          the sort order for YouTube Analytics data
      - in: query
        name: start-date
        description: The start date for fetching YouTube Analytics data
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Reports
  /subscriptions:
    get:
      summary: Get Subscriptions
      description: Returns subscription resources that match the API request criteria.
      operationId: getSubscriptions
      x-api-path-slug: subscriptions-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies a YouTube channel ID
      - in: query
        name: forChannelId
        description: The forChannelId parameter specifies a comma-separated list of
          channel IDs
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          subscription ID(s) for the resource(s) that are being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to retrieve a feed of the authenticated
          users subscriptions
      - in: query
        name: myRecentSubscribers
        description: Set this parameters value to true to retrieve a feed of the subscribers
          of the authenticated user in reverse chronological order (newest first)
      - in: query
        name: mySubscribers
        description: Set this parameters value to true to retrieve a feed of the subscribers
          of the authenticated user in no particular order
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: order
        description: The order parameter specifies the method that will be used to
          sort resources in the API response
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more subscription resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
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