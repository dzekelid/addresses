---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Put Users User Addresses User Address
  description: Updates a UserAddress with the given id.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/addresses:
    get:
      summary: Get Users User Addresses
      description: Retrieves a set of UserAddress objects associated to a User.
      operationId: getUsersUserAddresses
      x-api-path-slug: usersuser-idaddresses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
    post:
      summary: Post Users User Addresses
      description: Creates a new UserAddress.
      operationId: postUsersUserAddresses
      x-api-path-slug: usersuser-idaddresses-post
      parameters:
      - in: query
        name: city
      - in: query
        name: country_id
      - in: query
        name: first_line
      - in: query
        name: name
      - in: query
        name: second_line
      - in: query
        name: state
      - in: query
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
  /users/{user_id}/addresses/{user_address_id}:
    get:
      summary: Get Users User Addresses User Address
      description: Retrieves a UserAddress by id.
      operationId: getUsersUserAddressesUserAddress
      x-api-path-slug: usersuser-idaddressesuser-address-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
      - User
      - Address
    put:
      summary: Put Users User Addresses User Address
      description: Updates a UserAddress with the given id.
      operationId: putUsersUserAddressesUserAddress
      x-api-path-slug: usersuser-idaddressesuser-address-id-put
      parameters:
      - in: query
        name: city
      - in: query
        name: country_id
      - in: query
        name: first_line
      - in: query
        name: name
      - in: query
        name: second_line
      - in: query
        name: state
      - in: query
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
      - User
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