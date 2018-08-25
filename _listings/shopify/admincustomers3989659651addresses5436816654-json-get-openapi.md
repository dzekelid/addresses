---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get a single customers address
  description: Get a single customers address.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/customers/3989659651/addresses.json:
    get:
      summary: Get all of a customer's addresses
      description: Get all of a customer's addresses.
      operationId: getAdminCustomers3989659651Addresses.json
      x-api-path-slug: admincustomers3989659651addresses-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customers
      - Addresses
    post:
      summary: Creating a new address for a customer
      description: Creating a new address for a customer.
      operationId: postAdminCustomers3989659651Addresses.json
      x-api-path-slug: admincustomers3989659651addresses-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Creating
      - New
      - Addressa
      - Customer
  /admin/customers/3989659651/addresses/set.json:
    put:
      summary: destroying multiple customer addresses
      description: Destroying multiple customer addresses.
      operationId: putAdminCustomers3989659651AddressesSet.json
      x-api-path-slug: admincustomers3989659651addressesset-json-put
      parameters:
      - in: query
        name: address_ids[]
      - in: header
        name: Content-Type
      - in: query
        name: operation
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Destroying
      - Multiple
      - Customer
      - Addresses
  /admin/customers/3989659651/addresses/5484465742.json:
    delete:
      summary: Removing a customers address
      description: Removing a customers address.
      operationId: deleteAdminCustomers3989659651Addresses5484465742.json
      x-api-path-slug: admincustomers3989659651addresses5484465742-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Removing
      - Customers
      - Address
  /admin/customers/search.json:
    get:
      summary: Get all customers with an address in the Brazil
      description: Get all customers with an address in the brazil.
      operationId: getAdminCustomersSearch.json
      x-api-path-slug: admincustomerssearch-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customers
      - Address
      - In
      - Brazil
  /admin/customers/3989659651/addresses/5436816654/default.json:
    put:
      summary: assigning a new default address to a customer
      description: Assigning a new default address to a customer.
      operationId: putAdminCustomers3989659651Addresses5436816654Default.json
      x-api-path-slug: admincustomers3989659651addresses5436816654default-json-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Assigning
      - New
      - Default
      - Address
      - To
      - Customer
  /admin/customers/3989659651/addresses/5436816654.json:
    get:
      summary: Get a single customers address
      description: Get a single customers address.
      operationId: getAdminCustomers3989659651Addresses5436816654.json
      x-api-path-slug: admincustomers3989659651addresses5436816654-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Customers
      - Address
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