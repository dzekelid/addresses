swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
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
    get:
      summary: Get an list of Addresses
      description: Get an list of addresses.
      operationId: V2CustomersAddressesByCustomerIDGet2
      x-api-path-slug: v2customerscustomeridaddresses-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresseses