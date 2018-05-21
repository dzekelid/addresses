---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 1
info:
  title: Etsy
  description: bring-etsys-handmade-marketplace-and-community-into-your-apps
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
    delete:
      summary: Delete Users User Addresses User Address
      description: Deletes the UserAddress with the given id.
      operationId: deleteUsersUserAddressesUserAddress
      x-api-path-slug: usersuser-idaddressesuser-address-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
      - User
      - Address
---