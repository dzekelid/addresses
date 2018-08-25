---
swagger: "2.0"
x-collection-name: Tropo
x-complete: 0
info:
  title: Tropo Get Applications Appid Addresses
  description: Get applications appid addresses.
  version: v1
host: api.tropo.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /applications/{AppId}/addresses:
    delete:
      summary: Delete Applications Appid Addresses
      description: Delete applications appid addresses.
      operationId: deleteApplicationsAppAddresses
      x-api-path-slug: applicationsappidaddresses-delete
      parameters:
      - in: path
        name: AppId
      - in: query
        name: applicationId
      responses:
        200:
          description: OK
      tags:
      - Applications
      - AppId
      - Addresses
    get:
      summary: Get Applications Appid Addresses
      description: Get applications appid addresses.
      operationId: getApplicationsAppAddresses
      x-api-path-slug: applicationsappidaddresses-get
      parameters:
      - in: path
        name: AppId
      - in: query
        name: applicationId
      responses:
        200:
          description: OK
      tags:
      - Applications
      - AppId
      - Addresses
    post:
      summary: Post Applications Appid Addresses
      description: Post applications appid addresses.
      operationId: postApplicationsAppAddresses
      x-api-path-slug: applicationsappidaddresses-post
      parameters:
      - in: path
        name: AppId
      - in: query
        name: applicationId
      - in: query
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Applications
      - AppId
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