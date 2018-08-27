---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List warehouse addresses
  description: List warehouse addresses. The ID of the warehouse must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/addresses/{addressTypeId?}:
    get:
      summary: List addresses that are linked with contacts
      description: Lists addresses of the contact. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactAddressesAddresstype
      x-api-path-slug: restaccountscontactscontactidaddressesaddresstypeid-get
      parameters:
      - in: path
        name: addressTypeId?
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Addresses
      - That
      - Are
      - Linked
      - Contacts
  /rest/orders/{orderId}/addresses/{relationTypeId?}:
    get:
      summary: List order addresses
      description: Lists order addresses. The ID of the order must be specified.
      operationId: getRestOrdersOrderAddressesRelationtype
      x-api-path-slug: restordersorderidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: relationTypeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Addresses
  /rest/stockmanagement/warehouses/{warehouseId}/addresses/{relationTypeId?}:
    get:
      summary: List warehouse addresses
      description: List warehouse addresses. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseAddressesRelationtype
      x-api-path-slug: reststockmanagementwarehouseswarehouseidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: relationTypeId?
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
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