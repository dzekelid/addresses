swagger: "2.0"
x-collection-name: ParetoNetwork
x-complete: 1
info:
  title: PARETO NETWORK API
  description: the-pareto-network-api-is-used-by-sentinels-to-catalogue-and-relay-information-between-nodes--interacting-with-a-pareto-sentinel-uses-this-standardized-restful-api--authentication-is-done-using-a-json-web-token-jwt-stored-as-a-secure-browser-cookie--any-restful-client-will-need-to-set-the-cookie--here-is-a-tutorial-for-getting-the-initial-cookie-httpsblog-pareto-networkhowtousetheparetosentinelapi434afb75aace
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