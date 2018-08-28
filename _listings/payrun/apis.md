---
name: PayRun
x-slug: payrun
description: An open, scalable, transparent and HMRC accredited payroll API. Put the
  power of payroll into your application today.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
x-kinRank: "7"
x-alexaRank: "0"
tags: Relative StreamRank
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/apis.md
specificationVersion: "0.14"
apis:
- name: Pay Run.IO - Gets all employers
  x-api-slug: employers-get
  description: Gets links to all employers contained under the authorised application
    scope
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/employers-get-openapi.md
- name: Pay Run.IO - Get health check status
  x-api-slug: healthcheck-get
  description: Returns the health status of the application
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/healthcheck-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/healthcheck-get-openapi.md
- name: Pay Run.IO - Get all PayRun jobs
  x-api-slug: jobspayruns-get
  description: Gets all the pay run jobs
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/jobspayruns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/jobspayruns-get-openapi.md
- name: Pay Run.IO - Get the DPS job progress
  x-api-slug: jobsdpsjobidprogress-get
  description: Return the the DPS job progress
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/jobsdpsjobidprogress-get-openapi.md
- name: Pay Run.IO - Get the query result
  x-api-slug: query-post
  description: Get the results for the specified query
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/query-post-openapi.md
- name: Pay Run.IO - Get the RTI job progress
  x-api-slug: jobsrtijobidprogress-get
  description: Return the the RTI job progress
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/jobsrtijobidprogress-get-openapi.md
- name: Pay Run.IO - Get the RTI job status
  x-api-slug: jobsrtijobidstatus-get
  description: Return the the RTI job status
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/jobsrtijobidstatus-get-openapi.md
- name: Pay Run.IO - Gets all reports
  x-api-slug: reports-get
  description: Get links to all saved report definitions under authorised application
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/reports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/reports-get-openapi.md
- name: Pay Run.IO - Get a list of all available schemas
  x-api-slug: schemas-get
  description: Returns a collection of links to all the available data object schemas
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/schemas-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/schemas-get-openapi.md
- name: Pay Run.IO - Get employees with tag
  x-api-slug: employeremployeridemployeestagtagid-get
  description: Gets the employees with the tag
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/payrun/employeremployeridemployeestagtagid-get-openapi.md
x-common:
- type: x-website
  url: http://www.payrun.io
- type: x-api-gallery
  url: http://paypal.api.gallery.streamdata.io
- type: x-api-stack
  url: http://payrun.stack.network
- type: x-documentation
  url: https://developer.payrun.io/docs/home/index.html
- type: x-email
  url: support@payrun.io
- type: x-email
  url: info@payrun.io
- type: x-twitter
  url: https://twitter.com/PayRun_io
- type: x-website
  url: http://api.test.payrun.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---