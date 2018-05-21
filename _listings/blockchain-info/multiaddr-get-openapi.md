---
swagger: "2.0"
x-collection-name: Blockchain Info
x-complete: 0
info:
  title: Blockchain Info Multi Adress
  description: Returns multiple addresses
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rawaddr/{bitcoin_address}:
    get:
      summary: Raw Address
      description: Returns a single blockchain address.
      operationId: getRawAddress
      x-api-path-slug: rawaddrbitcoin-address-get
      parameters:
      - in: path
        name: bitcoin_address
        description: The bitcoin address
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Addresses
  /multiaddr:
    get:
      summary: Multi Adress
      description: Returns multiple addresses
      operationId: getMultipleAddresses
      x-api-path-slug: multiaddr-get
      parameters:
      - in: query
        name: active
        description: Multiple addresses divided by | Address can be base58 or xpub
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
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