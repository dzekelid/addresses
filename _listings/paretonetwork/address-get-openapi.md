---
swagger: "2.0"
x-collection-name: ParetoNetwork
x-complete: 0
info:
  title: Pareto Get the information of the current user
  description: Get the information of the current user. The current user is fetched
    using the auth cookie.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /address:
    get:
      summary: Get the information of the current user
      description: Get the information of the current user. The current user is fetched
        using the auth cookie.
      operationId: getAddress
      x-api-path-slug: address-get
      responses:
        200:
          description: OK
      tags:
      - Address
  /address/{address}:
    get:
      summary: Get the information of a specific user
      description: Get the information of a specific user.
      operationId: getAddressAddress
      x-api-path-slug: addressaddress-get
      parameters:
      - in: path
        name: address
        description: address to use
      responses:
        200:
          description: OK
      tags:
      - Address
      - Address
  /userinfo/{address}:
    get:
      summary: Get the profile of a specific user
      description: Get the profile of a specific user.
      operationId: getUserinfoAddress
      x-api-path-slug: userinfoaddress-get
      parameters:
      - in: path
        name: address
        description: address to use
      responses:
        200:
          description: OK
      tags:
      - Userinfo
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