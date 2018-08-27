swagger: "2.0"
x-collection-name: PayRun
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Templates/address:
    get:
      summary: Gets the address template
      description: Return the address data object template
      operationId: GetAddressTemplate
      x-api-path-slug: templatesaddress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Address
      - Template