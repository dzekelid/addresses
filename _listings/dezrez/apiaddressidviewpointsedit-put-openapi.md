---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Edits one or more ViewPoints of an address
  version: 1.0.0
  description: Edits one or more viewpoints of an address.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/suggest:
    get:
      summary: Search for properties/addresses that match the specified search criteria
      description: Search for properties/addresses that match the specified search
        criteria.
      operationId: Property_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumberBydataContract.s
      x-api-path-slug: apipropertysuggest-get
      parameters:
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: query
        name: dataContract.suggestType
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchproperties
      - Addresses
      - That
      - Match
      - Specified
      - Search
      - Criteria
  /api/address/{id}:
    get:
      summary: Get an address by its Id
      description: Get an address by its id.
      operationId: Address_GetByid
      x-api-path-slug: apiaddressid-get
      parameters:
      - in: path
        name: id
        description: The id of the address to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Address
      - By
      - Its
      - Id
  /api/address/{id}/viewpoints/edit:
    put:
      summary: Edits one or more ViewPoints of an address
      description: Edits one or more viewpoints of an address.
      operationId: Address_EditViewPointsByidBypoints
      x-api-path-slug: apiaddressidviewpointsedit-put
      parameters:
      - in: path
        name: id
        description: The Id of the address to update
      - in: body
        name: points
        description: One or more ViewPoints to edit
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Edits
      - More
      - ViewPoints
      - Of
      - Address
  /api/address/{id}/viewpoints/remove:
    put:
      summary: Removes one or more ViewPoints of an address
      description: Removes one or more viewpoints of an address.
      operationId: Address_RemoveViewPointsByidByviewpointIds
      x-api-path-slug: apiaddressidviewpointsremove-put
      parameters:
      - in: path
        name: id
        description: The Id of the address to update
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: viewpointIds
        description: One or more ViewPoints Ids to remove
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Removes
      - More
      - ViewPoints
      - Of
      - Address
  /api/credentials/emailsync/usernamepassword:
    post:
      summary: "Creates or Updates Email Sync Security Credentials\r\nThis also uses
        the credentials to do a quick check and see if they are working\r\nit will
        throw an internal server error if there is an issue with the connection\r\nbut
        this may be the server address (s"
      description: "Creates or updates email sync security credentials\r\nthis also
        uses the credentials to do a quick check and see if they are working\r\nit
        will throw an internal server error if there is an issue with the connection\r\nbut
        this may be the server address (s."
      operationId: Credentials_UpsertEmailSyncUsernamePasswordBycredentialDataContract
      x-api-path-slug: apicredentialsemailsyncusernamepassword-post
      parameters:
      - in: body
        name: credentialDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Email
      - Sync
      - Security
      - "Credentials\r\nThis"
      - Also
      - Uses
      - Credentials
      - To
      - Do
      - Quick
      - Check
      - See
      - If
      - They
      - Are
      - "Working\r\nIt"
      - Will
      - Throw
      - Internal
      - Server
      - Error
      - If
      - There
      - Is
      - Issue
      - "Connection\r\nBut"
      - This
      - May
      - Be
      - Server
      - Address
      - (s
  /api/people/findbyemail:
    get:
      summary: Returns a list of people that have the supplied email address.
      description: Returns a list of people that have the supplied email address..
      operationId: People_GetPeopleWithEmailAddressByemailAddress
      x-api-path-slug: apipeoplefindbyemail-get
      parameters:
      - in: query
        name: emailAddress
        description: The email address
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - People
      - That
      - Have
      - Supplied
      - Email
      - Address
  /api/property/{id}/updateaddress:
    put:
      summary: A command driven endpoint to Update a property address.
      description: A command driven endpoint to update a property address..
      operationId: Property_UpdateAddressByidByaddressDataContract
      x-api-path-slug: apipropertyidupdateaddress-put
      parameters:
      - in: body
        name: addressDataContract
        description: The address data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - ""
      - Property
      - Address
  /api/address/{id}/centerpoint:
    put:
      summary: Update the Center Point for an Address
      description: Update the center point for an address.
      operationId: Address_UpdateCenterPointByidByupdateCommand
      x-api-path-slug: apiaddressidcenterpoint-put
      parameters:
      - in: path
        name: id
        description: The Id of the address to update
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updateCommand
        description: The point details which will be updated on the address
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Center
      - Pointan
      - Ress
  /api/address/{id}/viewpoints/add:
    put:
      summary: Adds one or more View Points for an Address
      description: Adds one or more view points for an address.
      operationId: Address_AddViewPointsByidByviewPoints
      x-api-path-slug: apiaddressidviewpointsadd-put
      parameters:
      - in: path
        name: id
        description: The Id of the address to update
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: viewPoints
        description: One or more viewpoints to add
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - More
      - View
      - Pointsan
      - Ress
  /api/people/{id}/addaddress:
    put:
      summary: Add an Address to a Person
      description: Add an address to a person.
      operationId: People_AddAddressByidByaddress
      x-api-path-slug: apipeopleidaddaddress-put
      parameters:
      - in: body
        name: address
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Ress
      - To
      - Person
  /api/people/{id}/removeaddress/{addressId}:
    put:
      summary: Remove an Address from a Person
      description: Remove an address from a person.
      operationId: People_RemoveAddressByidByaddressId
      x-api-path-slug: apipeopleidremoveaddressaddressid-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Ress
      - From
      - Person
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