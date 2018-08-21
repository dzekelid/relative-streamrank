---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Provides summary information for all of a location's items.
  description: Provides summary information for all of a location's items.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/inventory:
    get:
      summary: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      description: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      operationId: ListInventory
      x-api-path-slug: v1location-idinventory-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of inventory entries to return in a single
          response
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Inventory
      - Information
      - Of
      - Merchants
      - Inventory-enabled
      - Item
      - Variations
  /v1/{location_id}/items:
    get:
      summary: Provides summary information for all of a location's items.
      description: Provides summary information for all of a location's items.
      operationId: ListItems
      x-api-path-slug: v1location-iditems-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: path
        name: location_id
        description: The ID of the location to list items for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Locations
      - Items
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