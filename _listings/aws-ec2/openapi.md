---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UnassignIpv6Addresses:
    get:
      summary: Unassign Ipv6 Addresses
      description: Unassigns one or more IPv6 addresses from a network interface.
      operationId: unassignipv6addresses
      x-api-path-slug: actionunassignipv6addresses-get
      parameters:
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: PrivateIpAddress.N
        description: The secondary private IP addresses to unassign from the network
          interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - IPv6 Addresses
---