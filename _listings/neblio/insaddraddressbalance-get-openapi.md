---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Returns address balance in sats
  description: Returns NEBL address balance in satoshis
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ins/addr/{address}:
    get:
      summary: Returns address object
      description: Returns NEBL address object containing information on a specific
        address
      operationId: getAddress
      x-api-path-slug: insaddraddress-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Object
  /ins/addr/{address}/balance:
    get:
      summary: Returns address balance in sats
      description: Returns NEBL address balance in satoshis
      operationId: getAddressBalance
      x-api-path-slug: insaddraddressbalance-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Balance
      - In
      - Sats
  /ins/addr/{address}/unconfirmedBalance:
    get:
      summary: Returns address unconfirmed balance in sats
      description: Returns NEBL address unconfirmed balance in satoshis
      operationId: getAddressUnconfirmedBalance
      x-api-path-slug: insaddraddressunconfirmedbalance-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Unconfirmed
      - Balance
      - In
      - Sats
  /ins/addr/{address}/totalReceived:
    get:
      summary: Returns total received by address in sats
      description: Returns total NEBL received by address in satoshis
      operationId: getAddressTotalReceived
      x-api-path-slug: insaddraddresstotalreceived-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Total
      - Received
      - By
      - Address
      - In
      - Sats
  /ins/addr/{address}/utxo:
    get:
      summary: Returns all UTXOs at a given address
      description: Returns information on each Unspent Transaction Output contained
        at an address
      operationId: getAddressUtxos
      x-api-path-slug: insaddraddressutxo-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - ""
      - UTXOs
      - At
      - Given
      - Address
  /ins/addr/{address}/totalSent:
    get:
      summary: Returns total sent by address in sats
      description: Returns total NEBL sent by address in satoshis
      operationId: getAddressTotalSent
      x-api-path-slug: insaddraddresstotalsent-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Total
      - Sent
      - By
      - Address
      - In
      - Sats
  /ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: getTxs
      x-api-path-slug: instxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
  /testnet/ins/addr/{address}:
    get:
      summary: Returns address object
      description: Returns NEBL address object containing information on a specific
        address
      operationId: testnet_getAddress
      x-api-path-slug: testnetinsaddraddress-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Object
  /testnet/ins/addr/{address}/balance:
    get:
      summary: Returns address balance in sats
      description: Returns NEBL address balance in satoshis
      operationId: testnet_getAddressBalance
      x-api-path-slug: testnetinsaddraddressbalance-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Balance
      - In
      - Sats
  /testnet/ins/addr/{address}/unconfirmedBalance:
    get:
      summary: Returns address unconfirmed balance in sats
      description: Returns NEBL address unconfirmed balance in satoshis
      operationId: testnet_getAddressUnconfirmedBalance
      x-api-path-slug: testnetinsaddraddressunconfirmedbalance-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Unconfirmed
      - Balance
      - In
      - Sats
  /testnet/ins/addr/{address}/totalReceived:
    get:
      summary: Returns total received by address in sats
      description: Returns total NEBL received by address in satoshis
      operationId: testnet_getAddressTotalReceived
      x-api-path-slug: testnetinsaddraddresstotalreceived-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Total
      - Received
      - By
      - Address
      - In
      - Sats
  /testnet/ins/addr/{address}/utxo:
    get:
      summary: Returns all UTXOs at a given address
      description: Returns information on each Unspent Transaction Output contained
        at an address
      operationId: testnet_getAddressUtxos
      x-api-path-slug: testnetinsaddraddressutxo-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - ""
      - UTXOs
      - At
      - Given
      - Address
  /testnet/ins/addr/{address}/totalSent:
    get:
      summary: Returns total sent by address in sats
      description: Returns total NEBL sent by address in satoshis
      operationId: testnet_getAddressTotalSent
      x-api-path-slug: testnetinsaddraddresstotalsent-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Total
      - Sent
      - By
      - Address
      - In
      - Sats
  /testnet/ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: testnet_getTxs
      x-api-path-slug: testnetinstxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
  /testnet/faucet:
    get:
      summary: Withdraws testnet NEBL to the specified address
      description: Withdraw testnet NEBL to your Neblio Testnet address. By default
        amount is 1500000000 or 15 NEBL and has a max of 50 NEBL. Only 2 withdrawals
        allowed per 24 hour period.
      operationId: testnet_getFaucet
      x-api-path-slug: testnetfaucet-get
      parameters:
      - in: query
        name: address
        description: Your Neblio Testnet Address
      - in: query
        name: amount
        description: Amount of NEBL to withdrawal in satoshis
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Withdraws
      - Testnet
      - NEBL
      - To
      - Specified
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