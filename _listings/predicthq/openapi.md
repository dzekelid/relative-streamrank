---
swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 1
info:
  title: PredictHQ API
  description: todo-add-description
  version: 1.0.0
host: api.predicthq.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/events/:
    get:
      summary: Retrieve All Events
      description: Use the below parameters to search and filter all events that are
        available to your account.
      operationId: V1EventsGet
      x-api-path-slug: v1events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/places/:
    get:
      summary: Search Places
      description: |-
        Use the below parameters to search and filter all places. Places are sorted by relevance (location or text query proximity).

        A search requires at least one of the `q`, `id`, `country` or `location` parameters.
      operationId: V1PlacesGet
      x-api-path-slug: v1places-get
      responses:
        200:
          description: OK
      tags:
      - Places
  /v1/signals/:
    get:
      summary: Retrieve All Signals
      description: It's easy to get a list of all Signals that are associated with
        your account.
      operationId: V1SignalsGet
      x-api-path-slug: v1signals-get
      responses:
        200:
          description: OK
      tags:
      - Signals
  /v1/signals/{signal_id}/analysis/:
    get:
      summary: Retrieve Analysis
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
      operationId: V1SignalsAnalysisBySignalIdGet
      x-api-path-slug: v1signalssignal-idanalysis-get
      parameters:
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
      - Analysis
  /v1/signals/{signal_id}/dimensions/:
    get:
      summary: Retrieve All Dimensions
      description: This action returns a summary for each dimension of your Signal.
      operationId: V1SignalsDimensionsBySignalIdGet
      x-api-path-slug: v1signalssignal-iddimensions-get
      parameters:
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
      - Dimensions
---