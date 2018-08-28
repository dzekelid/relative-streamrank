swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/stats/transactions:
    get:
      summary: Transaction Stats
      description: Transaction stats.
      operationId: getTransactionsStats
      x-api-path-slug: apiv1statstransactions-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      - in: query
        name: interval
        description: Interval
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - Stats
  /api/v1/transactions:
    get:
      summary: Browse Transactions
      description: Browse transactions.
      operationId: listTransactions
      x-api-path-slug: apiv1transactions-get
      parameters:
      - in: query
        name: currency_code
        description: Three letter ISO currency code
      - in: query
        name: filter_text
        description: Filtering expression
      - in: query
        name: format
        description: Output format - supports csv value for this operation
      - in: query
        name: has_note
        description: Return only transactions with a note field set
      - in: query
        name: invoice_number
        description: Transaction invoice number
      - in: query
        name: key_or_custom_id
        description: Taxamo provided transaction key or custom id
      - in: query
        name: limit
        description: Limit (no more than 1000, defaults to 100)
      - in: query
        name: offset
        description: Offset
      - in: query
        name: order_date_from
        description: Order date from in yyyy-MM-dd format
      - in: query
        name: order_date_to
        description: Order date to in yyyy-MM-dd format
      - in: query
        name: original_transaction_key
        description: Taxamo provided original transaction key
      - in: query
        name: sort_reverse
        description: If true, results are sorted in descending order
      - in: query
        name: statuses
        description: Comma separated list of of transaction statuses
      - in: query
        name: tax_country_code
        description: Two letter ISO tax country code
      - in: query
        name: tax_country_codes
        description: Comma separated list of two letter ISO tax country codes
      - in: query
        name: total_amount_greater_than
        description: Return only transactions with total amount greater than given
          number
      - in: query
        name: total_amount_less_than
        description: Return only transactions with total amount less than a given
          number
      responses:
        200:
          description: OK
      tags:
      - Browse
      - Transactions