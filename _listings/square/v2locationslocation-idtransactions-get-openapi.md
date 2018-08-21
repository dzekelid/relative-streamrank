---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API ListTransactions
  description: |-
    Lists transactions for a particular location.

    Max results per [page](#paginatingresults): 50
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
  /v1/{location_id}/orders:
    get:
      summary: Provides summary information for a merchant's online store orders.
      description: Provides summary information for a merchant's online store orders.
      operationId: ListOrders
      x-api-path-slug: v1location-idorders-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list online store orders for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Informationa
      - Merchants
      - Online
      - Store
      - Orders
  /v1/{location_id}/pages:
    get:
      summary: Lists all of a location's Favorites pages in Square Register.
      description: Lists all of a location's Favorites pages in Square Register.
      operationId: ListPages
      x-api-path-slug: v1location-idpages-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list Favorites pages for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Favorites
      - Pages
      - In
      - Square
      - Register
  /v1/{location_id}/payments:
    get:
      summary: Provides summary information for all payments taken by a merchant or
        any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      description: Provides summary information for all payments taken by a merchant
        or any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      operationId: ListPayments
      x-api-path-slug: v1location-idpayments-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list payments for
      - in: query
        name: order
        description: The order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Payments
      - Taken
      - By
      - Merchant
      - Any
      - Of
      - Merchants
      - Mobile
      - Staff
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
      - ""
      - See
      - Date
      - Rangesdetails
      - Of
      - Inclusive
      - Exclusive
      - Dates
  /v1/{location_id}/settlements:
    get:
      summary: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      description: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      operationId: ListSettlements
      x-api-path-slug: v1location-idsettlements-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list settlements for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      - in: query
        name: status
        description: Provide this parameter to retrieve only settlements with a particular
          status (SENT or FAILED)
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Deposits
      - Withdrawals
      - Initiated
      - By
      - Square
      - To
      - Merchants
      - Bank
      - Account
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
  /v2/catalog/list:
    get:
      summary: ListCatalog
      description: |-
        Returns a list of [CatalogObject](#type-catalogobject)s that includes
        all objects of a set of desired types (for example, all [CatalogItem](#type-catalogitem)
        and [CatalogTax](#type-catalogtax) objects) in the catalog. The types parameter
        is specified as a comma-separated list of valid [CatalogObject](#type-catalogobject) types:
        `ITEM`, `ITEM_VARIATION`, `MODIFIER`, `MODIFIER_LIST`, `CATEGORY`, `DISCOUNT`, `TAX`.
      operationId: ListCatalog
      x-api-path-slug: v2cataloglist-get
      parameters:
      - in: query
        name: cursor
        description: The pagination cursor returned in the previous response
      - in: query
        name: types
        description: An optional case-insensitive, comma-separated list of object
          types to retrieve, for example`ITEM,ITEM_VARIATION,CATEGORY`
      responses:
        200:
          description: OK
      tags:
      - ListCatalog
  /v2/customers:
    get:
      summary: ListCustomers
      description: Lists a business's customers.
      operationId: ListCustomers
      x-api-path-slug: v2customers-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: query
        name: cursor
        description: A pagination cursor returned by a previous call to this endpoint
      responses:
        200:
          description: OK
      tags:
      - ListCustomers
  /v2/locations:
    get:
      summary: ListLocations
      description: |-
        Provides the details for all of a business's locations.

        Most other Connect API endpoints have a required `location_id` path parameter.
        The `id` field of the [`Location`](#type-location) objects returned by this
        endpoint correspond to that `location_id` parameter.
      operationId: v2.locations.get
      x-api-path-slug: v2locations-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      responses:
        200:
          description: OK
      tags:
      - ListLocations
  /v2/locations/{location_id}/transactions:
    get:
      summary: ListTransactions
      description: |-
        Lists transactions for a particular location.

        Max results per [page](#paginatingresults): 50
      operationId: ListTransactions
      x-api-path-slug: v2locationslocation-idtransactions-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in RFC 3339
          format
      - in: query
        name: cursor
        description: A pagination cursor returned by a previous call to this endpoint
      - in: query
        name: end_time
        description: The end of the requested reporting period, in RFC 3339 format
      - in: path
        name: location_id
        description: The ID of the location to list transactions for
      - in: query
        name: sort_order
        description: The order in which results are listed in the response (`ASC`
          foroldest first, `DESC` for newest first)
      responses:
        200:
          description: OK
      tags:
      - ListTransactions
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