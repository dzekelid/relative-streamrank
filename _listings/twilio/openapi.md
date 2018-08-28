swagger: "2.0"
x-collection-name: Twilio
x-complete: 1
info:
  title: Twilio
  description: twilio-is-a-cloud-communications-infrastructure-as-a-serviceiaas-company-based-in-san-francisco-california--twilio-allows-software-developers-to-programmatically-make-and-receive-phone-calls-and-send-and-receive-text-messages-using-its-web-service-apis--twilios-services-are-accessed-over-http-and-are-billed-based-on-usage-
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
  /Accounts/{AccountSid}/Conferences.{format}:
    get:
      summary: Get Conference Calls
      description: Returns a list of conferences within an account. The list includes
        pagingninformation.n
      operationId: returns-a-list-of-conferences-within-an-account-the-list-includes-paginginformation
      x-api-path-slug: accountsaccountsidconferences-format-get
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
      - Conference Calls
  /Accounts/{AccountSid}/Conferences/{ConferenceSid}/Participants.{format}:
    get:
      summary: Get Conference Call Participants
      description: Returns the list of participants in the conference identified byn{ConferenceSid}.n
      operationId: returns-the-list-of-participants-in-the-conference-identified-byconferencesid
      x-api-path-slug: accountsaccountsidconferencesconferencesidparticipants-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: ConferenceSid
        description: A 34 character string that uniquely identifies the conference
          call object
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Conference Calls
  /Accounts/{AccountSid}/Queues:
    get:
      summary: Get Queues
      description: Returns a list of queues within an account. The list includes pagingninformation.n
      operationId: returns-a-list-of-queues-within-an-account-the-list-includes-paginginformation
      x-api-path-slug: accountsaccountsidqueues-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Queues
  /Accounts/{AccountSid}/Recordings:
    get:
      summary: Get Recordings
      description: Returns a list of Recording resource representations, each representing
        anrecording generated during the course of a phone call.n
      operationId: returns-a-list-of-recording-resource-representations-each-representing-arecording-generated-during-t
      x-api-path-slug: accountsaccountsidrecordings-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Recordings
  /Accounts/{AccountSid}/Transcriptions:
    get:
      summary: Get Transcriptions
      description: Returns a set of Transcription resource representations that includes
        pagingninformation.n
      operationId: returns-a-set-of-transcription-resource-representations-that-includes-paginginformation
      x-api-path-slug: accountsaccountsidtranscriptions-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Transcriptions