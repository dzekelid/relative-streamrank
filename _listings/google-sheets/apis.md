---
name: Google Sheets
x-slug: google-sheets
description: 'Google Sheets is an online spreadsheet app that lets users create and
  format spreadsheets and simultaneously work with other people. Google Sheets isn&rsquo;t
  only for consumers: its used every day by businesses and schools to manage spreadsheet
  data. With the new Sheets API v4 and Sheets add-ons, that data can be accessed by
  code as well as users.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-sheets-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Relative StreamRank
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/google-sheets/apis.md
specificationVersion: "0.14"
apis:
- name: Google Sheets - Get Spreadsheet
  x-api-slug: spreadsheetsspreadsheetid-get
  description: |-
    Returns the spreadsheet at the given ID.
    The caller must specify the spreadsheet ID.

    By default, data within grids will not be returned.
    You can include grid data one of two ways:

    * Specify a field mask listing your desired fields using the `fields` URL
    parameter in HTTP

    * Set the includeGridData
    URL parameter to true.  If a field mask is set, the `includeGridData`
    parameter is ignored

    For large spreadsheets, it is recommended to retrieve only the specific
    fields of the spreadsheet that you want.

    To retrieve only subsets of the spreadsheet, use the
    ranges URL parameter.
    Multiple ranges can be specified.  Limiting the range will
    return only the portions of the spreadsheet that intersect the requested
    ranges. Ranges are specified using A1 notation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-sheets-icon.png
  humanURL: https://developers.google.com/sheets/
  baseURL: https://sheets.googleapis.com/v4/
  tags: Google APIs, Spreadsheets, Data, Documents, Stack Network, Stack, Productivity,
    API Service Provider, API Provider, Profiles, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relative-streamrank/master/_listings/google-sheets/spreadsheetsspreadsheetid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.service.management.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.sheets.stack.network
- type: x-documentation
  url: https://developers.google.com/sheets/api/
- type: x-guides
  url: https://developers.google.com/sheets/api/guides/concepts
- type: x-issues
  url: https://code.google.com/a/google.com/p/apps-api-issues/
- type: x-rate-limits
  url: https://developers.google.com/sheets/api/limits
- type: x-samples
  url: https://developers.google.com/sheets/api/samples/
- type: x-support
  url: https://developers.google.com/sheets/api/support
- type: x-website
  url: https://developers.google.com/sheets/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---