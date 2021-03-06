---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Post Accounts Email Addresses
  description: Adds a new email address as an alias for an account.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/email_addresses:
    get:
      summary: Get Accounts Email Addresses
      description: Lists email addresses used by an account.
      operationId: listAccountEmailAddresses_
      x-api-path-slug: accountsidemail-addresses-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
    post:
      summary: Post Accounts Email Addresses
      description: Adds a new email address as an alias for an account.
      operationId: addAccountEmailAddress_
      x-api-path-slug: accountsidemail-addresses-post
      parameters:
      - in: query
        name: email_address
        description: An email address
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
  /accounts/{id}/email_addresses/{email}:
    post:
      summary: Post Accounts Email Addresses Email
      description: Makes this email address the primary one for the account.
      operationId: Create_setAccountEmailAddressAsPrimary_
      x-api-path-slug: accountsidemail-addressesemail-post
      parameters:
      - in: path
        name: email
        description: One of the email addresses associated to the account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: primary
        description: Set to 1 to make this email address the primary one for the account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
      - Email
    delete:
      summary: Delete Accounts Email Addresses Email
      description: Removes an email address form the aliases of an account.
      operationId: removeAccountEmailAddress_
      x-api-path-slug: accountsidemail-addressesemail-delete
      parameters:
      - in: path
        name: email
        description: One of the email addresses associated to the account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
      - Email
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