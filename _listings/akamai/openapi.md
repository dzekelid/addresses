---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /diagnostic-tools/v1/verifycdnip:
    get:
      summary: Is This a CDN IP
      description: Is This a CDN IP
      operationId: diagnostictoolsv1verifycdnipip
      x-api-path-slug: diagnostictoolsv1verifycdnip-get
      parameters:
      - in: query
        name: ip
        description: IP Address you want to determine is included in the Akamai network
        type: string
      responses:
        200:
          description: OK
      tags:
      - Diagnostic
      - Tools
      - Verifycdnip
      - IP Addresses
      - CDN
---