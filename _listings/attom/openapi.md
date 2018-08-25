---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /allevents/detail:
    get:
      summary: Returns all the events that have occurred on a specific address.
      description: Get a detail of all the events on a specific property based on
        its address.
      operationId: getAllEventsDetailAddress
      x-api-path-slug: alleventsdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: API Security Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - ""
      - Events
      - That
      - Have
      - Occurred
      - "On"
      - Specific
      - Address
  /poi/street+address:
    get:
      summary: Returns POIs based on an address.
      description: This search returns a list of POI in proximity to an address.
      operationId: getPOISearchPoint
      x-api-path-slug: poistreetaddress-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: RecordLimit
        description: This is RecordLimit
      - in: query
        name: SearchDistance
        description: This is SearchDistance
      - in: query
        name: Sort
        description: This is for Sortable Columns
      - in: query
        name: StreetAddress
        description: This is the Point value
      responses:
        200:
          description: OK
      tags:
      - Returns
      - POIs
      - Based
      - "On"
      - Address
---