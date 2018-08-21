---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR List stations close to you or filter by search criteria
  description: |-
    This endpoint has two main use cases:

    - If no query parameters passed in, it returns a list of stations that are geographically closest to the calling client (based on GeoIP information)
    - If one or more query parameters are passed in, it performs a search of NPR stations that match those search criteria (not taking into account the client's physical location)

    Clients wanting to implement a 'Change Station' UI should use this endpoint to power their search. In most cases, you'll want to build a search interface that uses one of the 3 provided schemas: `lat` and `lon` (using e.g. the HTML5 Geolocation API), `city` and `state`, _or_ the generic `q` query which can accept a station name, call letters, network name, or zip code. Technically speaking, `q` can also take in either a city name or a state name, but using the `city` and `state` parameters together will yield more accurate geographic search results than `q={cityName}`.

    The `lat` and `lon` query parameters should always be passed in together (otherwise the API will return a 400 error), and if included in the query, they will take precedence over any other search criteria; that is, `lat` and `lon` will do a purely geographic search and not take into account `q`, `city` or `state`.

    Similarly, `city` and/or `state` will take precedence over (and ignore) `q`.

    If clients want to be able to offer multiple types of searches (e.g. 'Search for a station name, city or zipcode') using a *single* search input form, `q` should be used. But again, be aware that using `city` and `state` together will yield more accurate search results than `q={cityName}`.
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sponsorship/v2/ads:
    get:
      summary: Request DAAST sponsorship units
      description: |-
        **Not** for use by NPR One clients (for whom sponsorship is already integrated into the Listening Service), this endpoint is designed to be used by our other client applications to request sponsorship on behalf of a user. Sponsorship units are returned in the form of DAAST XML. It is worth noting that this endpoint attempts to always return XML, even in the case of exceptions.

        The default behavior of this endpoint is asynchronous; on an initial request, a call to our external sponsorship provider is placed on a queue, which is typically processed within 3 minutes. Once the sponsorship call is received and processed, the returned sponsorship units are placed in a cache on our server for the current user. Subsequent calls to this endpoint will return DAAST sponsorship units from this cache until tracking information is submitted, which removes the ad from the cache and will automatically request additional ads asynchronously if there are fewer than a certain number remaining in the cache.

        For development purposes, it's worth noting that there is currently no way to clear a user's cache without submitting some form of tracking.
      operationId: getAds
      x-api-path-slug: sponsorshipv2ads-get
      parameters:
      - in: query
        name: adCount
        description: How many sponsorship units to request in one call; if left unspecified,
          the default behavior is to return only 1
      - in: query
        name: forceResult
        description: Whether to force a synchronous call to our external sponsorship
          provider; the default behavior is asynchronous
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - Sponsorship
      - Advertising
  /listening/v2/recommendations:
    get:
      summary: Get a list of media for the logged-in user from NPR's recommendation
        engine
      description: |-
        This endpoint returns a list of audio recommendations. It is designed to be used for an initial list of recommendations, and then `GET /listening/v2/ratings?recommend=true` should be used for subsequent requests for recommendations.

        A fully-populated link to the ratings endpoint is returned with each individual recommendation and is located in the AudioItemDocument under the `links['recommendations']` object. The query parameters in this link should not be modified.
        Be sure to copy and send back the entire ratings object (RatingData), as new fields may be added to it in the future.
      operationId: getRecommendations
      x-api-path-slug: listeningv2recommendations-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: notifiedMediaId
        description: The user received a push notification about this media; if provided,
          the service will add this recommendation to the top of the list
      - in: query
        name: sharedMediaId
        description: This media was shared directly with the user; if provided, the
          service will add this recommendation to the top of the list
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - Recommendations
  /listening/v2/history:
    get:
      summary: Get recent ratings the logged-in user has submitted
      description: This endpoint provides the list of recently-rated audio recommendations
        that the logged-in user has consumed. Some rated recommendations are filtered,
        such as sponsorship and donation.
      operationId: getHistory
      x-api-path-slug: listeningv2history-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - History
  /listening/v2/ratings:
    post:
      summary: Collect new ratings for media previously recommended to the logged-in
        user
      description: |-
        This endpoint is the main mechanism for providing feedback from the user to NPR about the recommendations that are obtained from `GET /listening/v2/recommendations`.

        A fully-populated link to this endpoint is returned with each individual recommendation and is located in the AudioItemDocument under the `links['recommendations']` object. The query parameters in this link should not be modified.
        Be sure to copy and send back the entire ratings object (RatingData), as new fields may be added to it in the future.

        This endpoint can return a blank JSON.doc or AudioItemDocument depending on the `recommend=true|false` parameter. The `recommend=true` flag allows this endpoint to both receive ratings and send back recommendations in the same call.
      operationId: postRating
      x-api-path-slug: listeningv2ratings-post
      parameters:
      - in: body
        name: body
        description: A list of RatingData objects which contains data about ratings
          such as the id of the content, the rating value, elapsed time and more
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: recommend
        description: If set to `false`, this call will return a blank document; otherwise
          it will return a new recommendation object
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - Ratings
  /listening/v2/search/recommendations:
    get:
      summary: Get a list of recent audio and aggregation items associated with search
        terms
      description: In the schema shown below, SearchItemDocument is not an actual
        type of returned object; the object returned by a search will be either an
        AggregationAudioItemListDocument or an AudioItemDocument.
      operationId: getSearchRecommendations
      x-api-path-slug: listeningv2searchrecommendations-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: searchTerms
        description: Search terms to search on; can include URL-encoded punctuation
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - Search
      - Recommendations
  /stationfinder/v3/stations:
    get:
      summary: List stations close to you or filter by search criteria
      description: |-
        This endpoint has two main use cases:

        - If no query parameters passed in, it returns a list of stations that are geographically closest to the calling client (based on GeoIP information)
        - If one or more query parameters are passed in, it performs a search of NPR stations that match those search criteria (not taking into account the client's physical location)

        Clients wanting to implement a 'Change Station' UI should use this endpoint to power their search. In most cases, you'll want to build a search interface that uses one of the 3 provided schemas: `lat` and `lon` (using e.g. the HTML5 Geolocation API), `city` and `state`, _or_ the generic `q` query which can accept a station name, call letters, network name, or zip code. Technically speaking, `q` can also take in either a city name or a state name, but using the `city` and `state` parameters together will yield more accurate geographic search results than `q={cityName}`.

        The `lat` and `lon` query parameters should always be passed in together (otherwise the API will return a 400 error), and if included in the query, they will take precedence over any other search criteria; that is, `lat` and `lon` will do a purely geographic search and not take into account `q`, `city` or `state`.

        Similarly, `city` and/or `state` will take precedence over (and ignore) `q`.

        If clients want to be able to offer multiple types of searches (e.g. 'Search for a station name, city or zipcode') using a *single* search input form, `q` should be used. But again, be aware that using `city` and `state` together will yield more accurate search results than `q={cityName}`.
      operationId: searchStations
      x-api-path-slug: stationfinderv3stations-get
      parameters:
      - in: query
        name: city
        description: A city to look for stations from; intended to be paired with
          `state`
      - in: query
        name: lat
        description: A latitude value from a geographic coordinate system; only works
          if paired with `lon`
      - in: query
        name: lon
        description: A longitude value from a geographic coordinate system; only works
          if paired with `lat`
      - in: query
        name: No Name
      - in: query
        name: q
        description: Search terms to search on; can be a station name, network name,
          call letters, or zipcode
      - in: query
        name: state
        description: A state to look for stations from (using the 2-letter abbreviation);
          intended to be paired with `city`
      responses:
        200:
          description: OK
      tags:
      - News
      - Stationfinder
      - Stations
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