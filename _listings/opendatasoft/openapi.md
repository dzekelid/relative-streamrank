swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 1
info:
  title: OpenDataSoft
  description: opendatasoft-is-a-cloudbased-turnkey-platform-for-data-publishing-and-api-management--its-interface-is-intuitively-designed-to-empower-anyone-regardless-of-technical-skills-to-upload-easytounderstand-open-data-or-to-even-share-data-within-an-admi---
  version: 2.1.0
host: public.opendatasoft.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pages:
    get:
      summary: Get Pages
      description: List of all pages from this portal.
      operationId: getPages
      x-api-path-slug: pages-get
      responses:
        200:
          description: OK
      tags:
      - Pages
  /{source}/datasets:
    get:
      summary: Get Source Datasets
      description: |-
        List of available datasets, each with their endpoints, paginated.

        Links provided:
        * previous page
        * next page
        * last page
        * first page
      operationId: getDatasets
      x-api-path-slug: sourcedatasets-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets