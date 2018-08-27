---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Search for properties/addresses that match the specified search criteria
  version: 1.0.0
  description: Search for properties/addresses that match the specified search criteria.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/suggest:
    get:
      summary: Search for properties/addresses that match the specified search criteria
      description: Search for properties/addresses that match the specified search
        criteria.
      operationId: Property_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumberBydataContract.s
      x-api-path-slug: apipropertysuggest-get
      parameters:
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: query
        name: dataContract.suggestType
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchproperties
      - Addresses
      - That
      - Match
      - Specified
      - Search
      - Criteria
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---