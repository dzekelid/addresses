---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateElasticIp:
    get:
      summary: Associate Elastic IP
      description: Associates one of the stack's registered Elastic IP addresses with
        a specified instance.
      operationId: associateElasticIp
      x-api-path-slug: actionassociateelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The Elastic IP address
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Associate
      - Elastic
      - IP Addresses
  /?Action=DeregisterElasticIp:
    get:
      summary: Deregister Elastic IP
      description: Deregisters a specified Elastic IP address.
      operationId: deregisterElasticIp
      x-api-path-slug: actionderegisterelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Elastic
      - IP Addresses
  /?Action=DescribeElasticIps:
    get:
      summary: Describes Elastic IPs
      description: Describes Elastic IPs
      operationId: describeElasticIps
      x-api-path-slug: actiondescribeelasticips-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: Ips
        description: An array of Elastic IP addresses to be described
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describes
      - Elastic
      - IP Addressess
---