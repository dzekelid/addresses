---
swagger: "2.0"
x-collection-name: Blockchain
x-complete: 1
info:
  title: Blockchain Info
  description: use-blockchains-apis-at-no-cost-to-help-you-start-building-bitcoin-apps-
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
---