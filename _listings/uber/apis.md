---
name: Uber
x-slug: uber
description: The Uber API exposes a set of RESTful endpoints that enable your application
  to GET information such as time and price estimates about the products offered in
  a given location, request rides on behalf of authenticated users, and create ride
  reminders for users to take a ride at a specific time in the future.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11277-uber.jpg
x-kinRank: "9"
x-alexaRank: "1255"
tags: Relative StreamRank
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/uber/apis.md
specificationVersion: "0.14"
apis:
- name: Uber - Price Estimates
  x-api-slug: estimatesprice-get
  description: The Price Estimates endpoint returns an estimated price range for each
    product offered at a given location. The price estimate is provided as a formatted
    string with the full price range and the localized currency symbol.<br><br>The
    response also includes low and high estimates, and the [ISO 4217](http://en.wikipedia.org/wiki/ISO_4217)
    currency code for situations requiring currency conversion. When surge is active
    for a particular product, its surge_multiplier will be greater than 1, but the
    price estimate already factors in this multiplier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11277-uber.jpg
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1
  tags: Taxis, Cars, Autos, Automobile, API LIfeyclessss, Transportation, Stack Network,
    Stack, Mobile, Marketplace, Technology, internet, Transportation, Profiles, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/uber/estimatesprice-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/uber/estimatesprice-get-openapi.md
- name: Uber - Time Estimates
  x-api-slug: estimatestime-get
  description: The Time Estimates endpoint returns ETAs for all products offered at
    a given location, with the responses expressed as integers in seconds. We recommend
    that this endpoint be called every minute to provide the most accurate, up-to-date
    ETAs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11277-uber.jpg
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1
  tags: Taxis, Cars, Autos, Automobile, API LIfeyclessss, Transportation, Stack Network,
    Stack, Mobile, Marketplace, Technology, internet, Transportation, Profiles, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/uber/estimatestime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/uber/estimatestime-get-openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://raw.githubusercontent.com/picsoung/apis.json/master/uber.json
- type: x-api-gallery
  url: http://u.s..digital.registry.api.gallery.streamdata.io
- type: x-api-stack
  url: http://uber.stack.network
- type: x-blog
  url: https://medium.com/streamrblog
- type: x-blog
  url: https://medium.com/@UberPubPolicy
- type: x-blog
  url: https://devblog.uber.com/
- type: x-blog-rss
  url: https://medium.com/feed/@UberPubPolicy
- type: x-blog-rss
  url: https://devblog.uber.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/uber
- type: x-developer
  url: https://developer.uber.com/
- type: x-email
  url: change-dr@uber.com
- type: x-github
  url: https://github.com/uber
- type: x-linkedin
  url: https://www.linkedin.com/company/uber-com/
- type: x-transparency-report
  url: https://transparencyreport.uber.com/
- type: x-twitter
  url: https://twitter.com/uber_api
- type: x-twitter
  url: https://twitter.com/UberPubPolicy
- type: x-twitter
  url: https://twitter.com/Uber
- type: x-website
  url: https://uber.com
- type: x-website
  url: http://medium.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---