swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/addresses:
    get:
      summary: Get My Addresses
      description: See all addresses in your address book
      operationId: getMyAddresses
      x-api-path-slug: myaddresses-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
    post:
      summary: Post My Addresses
      description: Create a new address in your address book
      operationId: postMyAddresses
      x-api-path-slug: myaddresses-post
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
  /my/addresses/{address_id}:
    delete:
      summary: Delete My Addresses Address
      description: Delete an existing address in your address book
      operationId: deleteMyAddressesAddress
      x-api-path-slug: myaddressesaddress-id-delete
      parameters:
      - in: path
        name: address_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
      - Address
      - Id
    put:
      summary: Put My Addresses Address
      description: Update an existing address in your address book
      operationId: putMyAddressesAddress
      x-api-path-slug: myaddressesaddress-id-put
      parameters:
      - in: path
        name: address_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
      - Address
      - Id