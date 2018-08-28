---
name: Pingdom
x-slug: pingdom
description: Monitor your websites availability and performance for free with Pingdom
  and always be the first to know when your website is down. No installation required.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
x-kinRank: "7"
x-alexaRank: "5876"
tags: Relative StreamRank
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apis.md
specificationVersion: "0.14"
apis:
- name: Checks API - Get Check List
  x-api-slug: apiversionchecks-get
  description: Returns a list overview of all checks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionchecks-get-openapi.md
- name: Checks API - Get Checks
  x-api-slug: checks-get
  description: Gets a list of all checks that are visible to you as a user or a customer
    depending on the request context.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/checks-get-openapi.md
- name: Checks API - Get Checks Results
  x-api-slug: checkscheckidresultsmillisecondsutc-get
  description: Gets a specific check result by a numeric java timestamp.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/checkscheckidresultsmillisecondsutc-get-openapi.md
- name: Checks API - Get Checks Results
  x-api-slug: checkscheckidresults-get
  description: Gets the most recent check results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/checkscheckidresults-get-openapi.md
- name: Summary API - Get A Response Time / Uptime Average
  x-api-slug: apiversionsummary-averagecheckid-get
  description: Get the average time / uptime value for a specified check and time
    period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-averagecheckid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-averagecheckid-get-openapi.md
- name: Summary API - Get Response Time Averages For Each Hour Of The Day
  x-api-slug: apiversionsummary-hoursofdaycheckid-get
  description: Returns the average response time for each hour of the day (0-23) for
    a specific check over a selected time period. I.e. it shows you what an average
    day looks like during that time period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-hoursofdaycheckid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-hoursofdaycheckid-get-openapi.md
- name: Summary API - Get List of Outages
  x-api-slug: apiversionsummary-outagecheckid-get
  description: Get a list of status changes for a specified check and time period.
    If order is speficied to descending, the list is ordered by newest first. (Default
    is ordered by oldest first.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-outagecheckid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-outagecheckid-get-openapi.md
- name: Summary API - Get Intervals of Average Response Time and Uptime During a Given
    Interval
  x-api-slug: apiversionsummary-performancecheckid-get
  description: |-
    For a given interval in time, return a list of sub intervals with the given resolution. Useful for generating graphs. A sub interval may be a week,
         a day or an hour depending on the choosen resolution.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-performancecheckid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-performancecheckid-get-openapi.md
- name: Summary API - Get Active Probes For A Period
  x-api-slug: apiversionsummary-probescheckid-get
  description: Get a list of probes that performed tests for a specified check during
    a specified period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/456-pingdom.jpg
  humanURL: http://www.pingdom.com
  baseURL: https://api.pingdom.com//
  tags: Monitoring, Performance, SaaS, Technology, internet, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-probescheckid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/pingdom/apiversionsummary-probescheckid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://pinboard.api.gallery.streamdata.io
- type: x-api-stack
  url: http://pingdom.stack.network
- type: x-base
  url: https://api.pingdom.com
- type: x-blog
  url: http://royal.pingdom.com/
- type: x-blog-rss
  url: http://royal.pingdom.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/pingdom
- type: x-crunchbase
  url: https://crunchbase.com/organization/pingdom
- type: x-developer
  url: https://www.pingdom.com/features/api/
- type: x-email
  url: sales@pingdom.com
- type: x-github
  url: https://github.com/Pingdom
- type: x-linkedin
  url: https://www.linkedin.com/company/pingdom
- type: x-pricing
  url: https://www.pingdom.com/pricing
- type: x-twitter
  url: https://twitter.com/#!/pingdom
- type: x-website
  url: http://www.pingdom.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---