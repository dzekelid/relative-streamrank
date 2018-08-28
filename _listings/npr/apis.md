---
name: NPR
x-slug: npr
description: NPR delivers breaking national and world news. Also top stories from
  business, politics, health, science, technology, music, arts and culture. Subscribe
  to podcasts and RSS feeds.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
x-kinRank: "9"
x-alexaRank: "598"
tags: Relative StreamRank
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/apis.md
specificationVersion: "0.14"
apis:
- name: NPR One API Reference - Request DAAST sponsorship units
  x-api-slug: sponsorshipv2ads-get
  description: |-
    **Not** for use by NPR One clients (for whom sponsorship is already integrated into the Listening Service), this endpoint is designed to be used by our other client applications to request sponsorship on behalf of a user. Sponsorship units are returned in the form of DAAST XML. It is worth noting that this endpoint attempts to always return XML, even in the case of exceptions.

    The default behavior of this endpoint is asynchronous; on an initial request, a call to our external sponsorship provider is placed on a queue, which is typically processed within 3 minutes. Once the sponsorship call is received and processed, the returned sponsorship units are placed in a cache on our server for the current user. Subsequent calls to this endpoint will return DAAST sponsorship units from this cache until tracking information is submitted, which removes the ad from the cache and will automatically request additional ads asynchronously if there are fewer than a certain number remaining in the cache.

    For development purposes, it's worth noting that there is currently no way to clear a user's cache without submitting some form of tracking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/sponsorshipv2ads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/sponsorshipv2ads-get-openapi.md
- name: NPR One API Reference - Get a list of media for the logged-in user from NPR's
    recommendation engine
  x-api-slug: listeningv2recommendations-get
  description: |-
    This endpoint returns a list of audio recommendations. It is designed to be used for an initial list of recommendations, and then `GET /listening/v2/ratings?recommend=true` should be used for subsequent requests for recommendations.

    A fully-populated link to the ratings endpoint is returned with each individual recommendation and is located in the AudioItemDocument under the `links['recommendations']` object. The query parameters in this link should not be modified.
    Be sure to copy and send back the entire ratings object (RatingData), as new fields may be added to it in the future.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/listeningv2recommendations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/listeningv2recommendations-get-openapi.md
- name: NPR One API Reference - Get recent ratings the logged-in user has submitted
  x-api-slug: listeningv2history-get
  description: This endpoint provides the list of recently-rated audio recommendations
    that the logged-in user has consumed. Some rated recommendations are filtered,
    such as sponsorship and donation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/listeningv2history-get-openapi.md
- name: NPR One API Reference - Collect new ratings for media previously recommended
    to the logged-in user
  x-api-slug: listeningv2ratings-post
  description: |-
    This endpoint is the main mechanism for providing feedback from the user to NPR about the recommendations that are obtained from `GET /listening/v2/recommendations`.

    A fully-populated link to this endpoint is returned with each individual recommendation and is located in the AudioItemDocument under the `links['recommendations']` object. The query parameters in this link should not be modified.
    Be sure to copy and send back the entire ratings object (RatingData), as new fields may be added to it in the future.

    This endpoint can return a blank JSON.doc or AudioItemDocument depending on the `recommend=true|false` parameter. The `recommend=true` flag allows this endpoint to both receive ratings and send back recommendations in the same call.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/listeningv2ratings-post-openapi.md
- name: NPR One API Reference - Get a list of recent audio and aggregation items associated
    with search terms
  x-api-slug: listeningv2searchrecommendations-get
  description: In the schema shown below, SearchItemDocument is not an actual type
    of returned object; the object returned by a search will be either an AggregationAudioItemListDocument
    or an AudioItemDocument.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/listeningv2searchrecommendations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/listeningv2searchrecommendations-get-openapi.md
- name: NPR One API Reference - List stations close to you or filter by search criteria
  x-api-slug: stationfinderv3stations-get
  description: |-
    This endpoint has two main use cases:

    - If no query parameters passed in, it returns a list of stations that are geographically closest to the calling client (based on GeoIP information)
    - If one or more query parameters are passed in, it performs a search of NPR stations that match those search criteria (not taking into account the client's physical location)

    Clients wanting to implement a 'Change Station' UI should use this endpoint to power their search. In most cases, you'll want to build a search interface that uses one of the 3 provided schemas: `lat` and `lon` (using e.g. the HTML5 Geolocation API), `city` and `state`, _or_ the generic `q` query which can accept a station name, call letters, network name, or zip code. Technically speaking, `q` can also take in either a city name or a state name, but using the `city` and `state` parameters together will yield more accurate geographic search results than `q={cityName}`.

    The `lat` and `lon` query parameters should always be passed in together (otherwise the API will return a 400 error), and if included in the query, they will take precedence over any other search criteria; that is, `lat` and `lon` will do a purely geographic search and not take into account `q`, `city` or `state`.

    Similarly, `city` and/or `state` will take precedence over (and ignore) `q`.

    If clients want to be able to offer multiple types of searches (e.g. 'Search for a station name, city or zipcode') using a *single* search input form, `q` should be used. But again, be aware that using `city` and `state` together will yield more accurate search results than `q={cityName}`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/stationfinderv3stations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/npr/stationfinderv3stations-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://nfusion.solutions.api.gallery.streamdata.io
- type: x-api-stack
  url: http://npr.stack.network
- type: x-base
  url: http://api.npr.org/
- type: x-codecademy
  url: http://www.codecademy.com/tracks/npr
- type: x-crunchbase
  url: https://crunchbase.com/organization/npr
- type: x-crunchbase
  url: http://www.crunchbase.com/company/npr
- type: x-developer
  url: http://dev.npr.org/
- type: x-documentation
  url: http://dev.npr.org/#accessing-the-api
- type: x-email
  url: permissions@npr.org
- type: x-email
  url: ogcstaff@npr.org
- type: x-email
  url: employment@npr.org
- type: x-email
  url: careers@npr.org
- type: x-email
  url: kroc@npr.org
- type: x-email
  url: mediarelations@npr.org
- type: x-email
  url: sponsorship@npr.org
- type: x-email
  url: ashamblin@npr.org
- type: x-email
  url: giving@npr.org
- type: x-email
  url: giftplanning@npr.org
- type: x-email
  url: NPRDonorCommunications@npr.org
- type: x-getting-started
  url: http://dev.npr.org/#quick-start
- type: x-github
  url: https://github.com/npr
- type: x-selfservice-registration
  url: http://www.npr.org/templates/reg/
- type: x-terms-of-service
  url: http://www.npr.org/about-npr/179876898/terms-of-use
- type: x-twitter
  url: https://twitter.com/NPR
- type: x-twitter
  url: https://twitter.com/NPRTechTeam
- type: x-website
  url: http://npr.org
- type: x-website
  url: http://www.npr.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---