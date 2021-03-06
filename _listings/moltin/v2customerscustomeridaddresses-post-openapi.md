---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Create an Address
  description: Create an address.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/customers/{customerID}/addresses/{addressID}:
    get:
      summary: Get an Address
      description: Get an address.
      operationId: V2CustomersAddressesByCustomerIDAndAddressIDGet
      x-api-path-slug: v2customerscustomeridaddressesaddressid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: addressID
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
    put:
      summary: Update an Address
      description: Update an address.
      operationId: V2CustomersAddressesByCustomerIDAndAddressIDPut
      x-api-path-slug: v2customerscustomeridaddressesaddressid-put
      parameters:
      - in: header
        name: Accept
      - in: path
        name: addressID
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
    delete:
      summary: Delete an Address
      description: Delete an address.
      operationId: V2CustomersAddressesByCustomerIDAndAddressIDDelete
      x-api-path-slug: v2customerscustomeridaddressesaddressid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: addressID
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
  /v2/customers/{customerID}/addresses:
    post:
      summary: Create an Address
      description: Create an address.
      operationId: V2CustomersAddressesByCustomerIDPost
      x-api-path-slug: v2customerscustomeridaddresses-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
        description: Change default locale
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
        description: Change from default currency
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
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