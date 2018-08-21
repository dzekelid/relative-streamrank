---
swagger: "2.0"
x-collection-name: Uber
x-complete: 0
info:
  title: Uber Time Estimates
  description: The Time Estimates endpoint returns ETAs for all products offered at
    a given location, with the responses expressed as integers in seconds. We recommend
    that this endpoint be called every minute to provide the most accurate, up-to-date
    ETAs.
  version: 1.0.0
host: api.uber.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /estimates/price:
    get:
      summary: Price Estimates
      description: The Price Estimates endpoint returns an estimated price range for
        each product offered at a given location. The price estimate is provided as
        a formatted string with the full price range and the localized currency symbol.<br><br>The
        response also includes low and high estimates, and the [ISO 4217](http://en.wikipedia.org/wiki/ISO_4217)
        currency code for situations requiring currency conversion. When surge is
        active for a particular product, its surge_multiplier will be greater than
        1, but the price estimate already factors in this multiplier.
      operationId: the-price-estimates-endpoint-returns-an-estimated-price-range-for-each-product-offered-at-a-given-lo
      x-api-path-slug: estimatesprice-get
      parameters:
      - in: query
        name: end_latitude
        description: Latitude component of end location
      - in: query
        name: end_longitude
        description: Longitude component of end location
      - in: query
        name: start_latitude
        description: Latitude component of start location
      - in: query
        name: start_longitude
        description: Longitude component of start location
      responses:
        200:
          description: OK
      tags:
      - Transportation
  /estimates/time:
    get:
      summary: Time Estimates
      description: The Time Estimates endpoint returns ETAs for all products offered
        at a given location, with the responses expressed as integers in seconds.
        We recommend that this endpoint be called every minute to provide the most
        accurate, up-to-date ETAs.
      operationId: the-time-estimates-endpoint-returns-etas-for-all-products-offered-at-a-given-location-with-the-respo
      x-api-path-slug: estimatestime-get
      parameters:
      - in: query
        name: customer_uuid
        description: Unique customer identifier to be used for experience customization
      - in: query
        name: product_id
        description: Unique identifier representing a specific product for a given
          latitude & longitude
      - in: query
        name: start_latitude
        description: Latitude component of start location
      - in: query
        name: start_longitude
        description: Longitude component of start location
      responses:
        200:
          description: OK
      tags:
      - Transportation
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