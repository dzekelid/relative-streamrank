---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Get Calls
  description: Get Calls
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Usage/Records:
    get:
      summary: Get Account Usage Record
      description: Returns UsageRecords for all usage categories. The list includes
        pagingninformation.nBy default, the UsageRecords resource will return one
        UsageRecord forneach Category, representing all usage accrued all-time for
        the account.nYou can filter the usage Category or change the date-range over
        which usagenis counted using optional GET query parameters.n
      operationId: returns-usagerecords-for-all-usage-categories-the-list-includes-paginginformationby-default-the-usag
      x-api-path-slug: accountsaccountsidusagerecords-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Usage Records
  /Accounts/{AccountSid}/SMS/Messages.{format}:
    get:
      summary: GetSMSList
      description: GetSMSList
      operationId: getsmslist
      x-api-path-slug: accountsaccountsidsmsmessages-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
      responses:
        200:
          description: OK
      tags:
      - SMS Messages
  /Accounts/{AccountSid}/Messages.{format}:
    get:
      summary: Get Message Media
      description: Returns a list of messages associated with your account. The list
        includes paging information.
      operationId: returns-a-list-of-messages-associated-with-your-account-the-list-includes-paging-information
      x-api-path-slug: accountsaccountsidmessages-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /Accounts/{AccountSid}/Applications.{format}:
    get:
      summary: Get Applications
      description: Get Applications
      operationId: returns-a-list-of-application-resource-representations-each-representingan-application-within-your-a
      x-api-path-slug: accountsaccountsidapplications-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /Accounts/{AccountSid}/Calls.{format}:
    get:
      summary: Get Calls
      description: Get Calls
      operationId: getCalls
      x-api-path-slug: accountsaccountsidcalls-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Calls
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