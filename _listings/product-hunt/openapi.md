---
swagger: "2.0"
x-collection-name: Product Hunt
x-complete: 1
info:
  title: Product Hunt
  version: 1.0.0
host: api.producthunt.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories/{category}/posts:
    get:
      summary: Get Categories
      description: Get categories.
      operationId: getCategoriesCategoryAdds
      x-api-path-slug: categoriescategoryposts-get
      parameters:
      - in: path
        name: category
      - in: query
        name: days_ago
      responses:
        200:
          description: OK
      tags:
      - Categories
---