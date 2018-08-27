---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik Show an address
  description: "Show an individual address for an account.\nRegular bitcoin address
    can be used in place of address_id but the address has to be associated to the
    correct account.\n  \n*Important* Addresses should be considered one time use
    only."
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}/addresses:
    get:
      summary: List addresses
      description: |-
        Lists addresses for an account.

        *Important*: Addresses should be considered one time use only.
      operationId: lists-addresses-for-an-accountimportant-addresses-should-be-considered-one-time-use-only
      x-api-path-slug: accountsaccount-idaddresses-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Addresses
    post:
      summary: Create address
      description: "Creates a new address for an account. As all the arguments are
        optinal, it\u2019s possible just to do a empty POST which will create a new
        address. This is handy if you need to create new receive addresses for an
        account on-demand.\nAddresses can be created for all account types. With fiat
        accounts, funds will be received with Instant Exchange."
      operationId: creates-a-new-address-for-an-account-as-all-the-arguments-are-optinal-its-possible-just-to-do-a-empt
      x-api-path-slug: accountsaccount-idaddresses-post
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: body
        name: address_properties
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Address
  /accounts/{account_id}/addresses/{address_id}:
    get:
      summary: Show an address
      description: "Show an individual address for an account.\nRegular bitcoin address
        can be used in place of address_id but the address has to be associated to
        the correct account.\n  \n*Important* Addresses should be considered one time
        use only."
      operationId: show-an-individual-address-for-an-accountregular-bitcoin-address-can-be-used-in-place-of-address-id-
      x-api-path-slug: accountsaccount-idaddressesaddress-id-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: address_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Address
  /accounts/{account_id}/addresses/{address_id}/transactions:
    get:
      summary: "List address\u2019s transactions"
      description: list transactions that have been sent to a specific address. Regular
        bitcoin address can be used in place of address_id but the address has to
        be associated to the correct account.
      operationId: list-transactions-that-have-been-sent-to-a-specific-address-regular-bitcoin-address-can-be-used-in-p
      x-api-path-slug: accountsaccount-idaddressesaddress-idtransactions-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: address_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - "Address\u2019s"
      - Transactions
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