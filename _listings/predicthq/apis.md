---
name: PredictHQ
x-slug: predicthq
description: Event visibility yields higher returns & reduces operational costs. PredictHQ
  is the worlds largest source of intelligent event data making businesses smarter.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-predicthq.jpg
x-kinRank: "7"
x-alexaRank: "292227"
tags: Relative StreamRank
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/apis.md
specificationVersion: "0.14"
apis:
- name: PredictHQ API - Retrieve All Events
  x-api-slug: v1events-get
  description: Use the below parameters to search and filter all events that are available
    to your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-predicthq.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com//
  tags: SaaS, Technology, Events, API Provider, Profiles, Service API, Relative Data,
    Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1events-get-openapi.md
- name: PredictHQ API - Search Places
  x-api-slug: v1places-get
  description: |-
    Use the below parameters to search and filter all places. Places are sorted by relevance (location or text query proximity).

    A search requires at least one of the `q`, `id`, `country` or `location` parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-predicthq.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com//
  tags: SaaS, Technology, Events, API Provider, Profiles, Service API, Relative Data,
    Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1places-get-openapi.md
- name: PredictHQ API - Retrieve All Signals
  x-api-slug: v1signals-get
  description: It's easy to get a list of all Signals that are associated with your
    account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-predicthq.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com//
  tags: SaaS, Technology, Events, API Provider, Profiles, Service API, Relative Data,
    Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1signals-get-openapi.md
- name: PredictHQ API - Retrieve Analysis
  x-api-slug: v1signalssignal-idanalysis-get
  description: |-
    This action returns a complete analysis of your Signal, which includes what your actual figures were, what could be expected, and what was in excess in terms of **demand**, **lead time** and **duration** and can be explained using events. Note that lead time (`lead`) and duration (`span`) analysis are only available when an `initiated` and `completed` dates are provided with data points, respectively.

    To retrieve a list of events that we estimate impacted your business at a specific date in the past, use the `signal.id` and `signal.explain` parameters with the events endpoint.

    Alternatively, to retrieve a list of predicted events that we estimate will impact your business in the future, use the `signal.id` parameter and the date range you wish a prediction for using `active` or `start`.

    See the events endpoint for more details.

    The `significance` parameter corresponds to percentage of variation in your data that is considered normal when computing excess that can be attributed to events. If you were to look at a normal distribution, it would correspond to the percentage of values that lie within a band around the mean.

    As an example:
    - ~68.27% = 1 standard deviation from the mean
    - ~95.45% = 2 standard deviations from the mean
    - ~99.73% = 3 standard deviations from the mean

    A high `significance` means that only extreme spikes and troughs will be attributed to events. We use 50% as a default, which corresponds to ~0.68 standard deviations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-predicthq.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com//
  tags: SaaS, Technology, Events, API Provider, Profiles, Service API, Relative Data,
    Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1signalssignal-idanalysis-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1signalssignal-idanalysis-get-openapi.md
- name: PredictHQ API - Retrieve All Dimensions
  x-api-slug: v1signalssignal-iddimensions-get
  description: This action returns a summary for each dimension of your Signal.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-predicthq.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com//
  tags: SaaS, Technology, Events, API Provider, Profiles, Service API, Relative Data,
    Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1signalssignal-iddimensions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/predicthq/v1signalssignal-iddimensions-get-openapi.md
x-common:
- type: x-website
  url: http://www.predicthq.com/
- type: x-api-gallery
  url: http://postmark.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predicthq.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predicthq
- type: x-email
  url: support@predicthq.com
- type: x-email
  url: 8Bsupport@predicthq.com
- type: x-email
  url: notices@predicthq.com
- type: x-github
  url: https://github.com/predicthq
- type: x-linkedin
  url: PredictHQ
- type: x-twitter
  url: https://twitter.com/PredictHQ
- type: x-website
  url: https://developer.predicthq.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---