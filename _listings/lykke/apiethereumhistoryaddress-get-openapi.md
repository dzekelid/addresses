---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Ethereum History Address
  version: 1.0.0
  description: Get api ethereum history address.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/HotWallet/addresses/{destinationAddress}/{assetId}/validity:
    get:
      summary: Get API Hotwallet Addresses Destinationaddress Asset Vality
      description: Get api hotwallet addresses destinationaddress asset vality.
      operationId: AddressValidity
      x-api-path-slug: apihotwalletaddressesdestinationaddressassetidvalidity-get
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: destinationAddress
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Resses
      - Destinationaddress
      - Asset
      - Vality
  /api/Email/PrivateWalletAddress:
    post:
      summary: Add API Email Privatewalletaddress
      description: Add api email privatewalletaddress.
      operationId: ApiEmailPrivateWalletAddressPost
      x-api-path-slug: apiemailprivatewalletaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Privatewalletaddress
  /api/EmailMeWalletAddress:
    post:
      summary: Add API Emailmewalletaddress
      description: Add api emailmewalletaddress.
      operationId: ApiEmailMeWalletAddressPost
      x-api-path-slug: apiemailmewalletaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Emailmewalletaddress
  /api/Ethereum/history/{address}:
    get:
      summary: Get API Ethereum History Address
      description: Get api ethereum history address.
      operationId: ApiEthereumHistoryByAddressGet
      x-api-path-slug: apiethereumhistoryaddress-get
      parameters:
      - in: path
        name: address
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: count
      - in: query
        name: start
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - History
      - Ress
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