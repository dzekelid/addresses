---
swagger: "2.0"
x-collection-name: AWS Snowball
x-complete: 0
info:
  title: AWS Snowball API Describe Address
  version: 1.0.0
  description: |-
    Takes an AddressId and returns specific details about that address in the
          form of an Address object.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateAddress:
    get:
      summary: Create Address
      description: Creates an address for a Snowball to be shipped to.
      operationId: createAddress
      x-api-path-slug: actioncreateaddress-get
      parameters:
      - in: query
        name: Address
        description: The address that you want the Snowball shipped to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Addresses
  /?Action=DescribeAddress:
    get:
      summary: Describe Address
      description: |-
        Takes an AddressId and returns specific details about that address in the
              form of an Address object.
      operationId: describeAddress
      x-api-path-slug: actiondescribeaddress-get
      parameters:
      - in: query
        name: AddressId
        description: The automatically generated ID for a specific address
        type: string
      responses:
        200:
          description: OK
      tags:
      - Addresses
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