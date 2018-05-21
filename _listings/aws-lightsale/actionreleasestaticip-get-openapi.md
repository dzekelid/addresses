---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Release Static Ip
  version: 1.0.0
  description: Deletes a specific static IP from your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AllocateStaticIp:
    get:
      summary: Allocate Static Ip
      description: Allocates a static IP address.
      operationId: allocateStaticIp
      x-api-path-slug: actionallocatestaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=AttachStaticIp:
    get:
      summary: Attach Static Ip
      description: Attaches a static IP address to a specific Amazon Lightsail instance.
      operationId: attachStaticIp
      x-api-path-slug: actionattachstaticip-get
      parameters:
      - in: query
        name: instanceName
        description: The instance name to which you want to attach the static IP address
        type: string
      - in: query
        name: staticIpName
        description: The name of the static IP
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=DetachStaticIp:
    get:
      summary: Detach Static Ip
      description: |-
        Detaches a static IP from the Amazon Lightsail instance to which it is
              attached.
      operationId: detachStaticIp
      x-api-path-slug: actiondetachstaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP to detach from the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=GetStaticIp:
    get:
      summary: Get Static Ip
      description: Returns information about a specific static IP.
      operationId: getStaticIp
      x-api-path-slug: actiongetstaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP in Lightsail
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=GetStaticIps:
    get:
      summary: Get Static Ips
      description: Returns information about all static IPs in the user's account.
      operationId: getStaticIps
      x-api-path-slug: actiongetstaticips-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get static IPs      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=ReleaseStaticIp:
    get:
      summary: Release Static Ip
      description: Deletes a specific static IP from your account.
      operationId: releaseStaticIp
      x-api-path-slug: actionreleasestaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
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