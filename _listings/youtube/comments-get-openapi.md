---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Get Comments
  description: Returns a list of comments that match the API request parameters.
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
  /v1/jobs:
    get:
      summary: Get Jobs
      description: Lists jobs.
      operationId: getV1Jobs
      x-api-path-slug: v1jobs-get
      parameters:
      - in: query
        name: includeSystemManaged
        description: If set to true, also system-managed jobs will be returned; otherwise
          onlyuser-created jobs will be returned
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results the server should return
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
  /videos:
    get:
      summary: Get Videos
      description: Returns a list of videos that match the API request parameters.
      operationId: getVeos
      x-api-path-slug: videos-get
      parameters:
      - in: query
        name: chart
        description: The chart parameter identifies the chart that you want to retrieve
      - in: query
        name: hl
        description: The hl parameter instructs the API to retrieve localized resource
          metadata for a specific application language that the YouTube website supports
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          video ID(s) for the resource(s) that are being retrieved
      - in: query
        name: locale
        description: DEPRECATED
      - in: query
        name: maxHeight
        description: The maxHeight parameter specifies a maximum height of the embedded
          player
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: maxWidth
        description: The maxWidth parameter specifies a maximum width of the embedded
          player
      - in: query
        name: myRating
        description: Set this parameters value to like or dislike to instruct the
          API to only return videos liked or disliked by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more video resource properties that the API response will include
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to select a video
          chart available in the specified region
      - in: query
        name: videoCategoryId
        description: The videoCategoryId parameter identifies the video category for
          which the chart should be retrieved
      responses:
        200:
          description: OK
      tags:
      - Veos
  /activities:
    get:
      summary: Get Activities
      description: Returns a list of channel activity events that match the request
        criteria. For example, you can retrieve events associated with a particular
        channel, events associated with the user's subscriptions and Google+ friends,
        or the YouTube home page feed, which is customized for each user.
      operationId: getActivities
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies a unique YouTube channel ID
      - in: query
        name: home
        description: Set this parameters value to true to retrieve the activity feed
          that displays on the YouTube home page for the currently authenticated user
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to retrieve a feed of the authenticated
          users activities
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more activity resource properties that the API response will include
      - in: query
        name: publishedAfter
        description: The publishedAfter parameter specifies the earliest date and
          time that an activity could have occurred for that activity to be included
          in the API response
      - in: query
        name: publishedBefore
        description: The publishedBefore parameter specifies the date and time before
          which an activity must have occurred for that activity to be included in
          the API response
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return results
          for the specified country
      responses:
        200:
          description: OK
      tags:
      - Activities
  /channels:
    get:
      summary: Get Channels
      description: Returns a collection of zero or more channel resources that match
        the request criteria.
      operationId: getChannels
      x-api-path-slug: channels-get
      parameters:
      - in: query
        name: categoryId
        description: The categoryId parameter specifies a YouTube guide category,
          thereby requesting YouTube channels associated with that category
      - in: query
        name: forUsername
        description: The forUsername parameter specifies a YouTube username, thereby
          requesting the channel associated with that username
      - in: query
        name: hl
        description: The hl parameter should be used for filter out the properties
          that are not in the given language
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          channel ID(s) for the resource(s) that are being retrieved
      - in: query
        name: managedByMe
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to instruct the API to only
          return channels owned by the authenticated user
      - in: query
        name: mySubscribers
        description: Use the subscriptions
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more channel resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Channels
  /comments:
    get:
      summary: Get Comments
      description: Returns a list of comments that match the API request parameters.
      operationId: getComments
      x-api-path-slug: comments-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of comment
          IDs for the resources that are being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: parentId
        description: The parentId parameter specifies the ID of the comment for which
          replies should be retrieved
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more comment resource properties that the API response will include
      - in: query
        name: textFormat
        description: This parameter indicates whether the API should return comments
          formatted as HTML or as plain text
      responses:
        200:
          description: OK
      tags:
      - Comments
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