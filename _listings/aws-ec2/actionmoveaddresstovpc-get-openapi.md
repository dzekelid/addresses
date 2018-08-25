---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Move Address To Vpc
  version: 1.0.0
  description: Moves an Elastic IP address from the EC2-Classic platform to the EC2-VPC
    platform.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssignIpv6Addresses:
    get:
      summary: Assign Ipv6 Addresses
      description: Assigns one or more IPv6 addresses to the specified network interface.
      operationId: assignipv6addresses
      x-api-path-slug: actionassignipv6addresses-get
      parameters:
      - in: query
        name: AllowReassignment
        description: Indicates whether to allow an IP address that is already assigned
          to another network interface or instance to be reassigned to the specified
          network interface
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: PrivateIpAddress.N
        description: One or more IP addresses to be assigned as a secondary private
          IP address to the network interface
        type: string
      - in: query
        name: SecondaryPrivateIpAddressCount
        description: The number of secondary IP addresses to assign to the network
          interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
  /?Action=AssignPrivateIpAddresses:
    get:
      summary: Assign Private Ip Addresses
      description: Assigns one or more secondary private IP addresses to the specified
        network interface.
      operationId: assignprivateipaddresses
      x-api-path-slug: actionassignprivateipaddresses-get
      parameters:
      - in: query
        name: DeviceIndex
        description: The index of the device for the network interface attachment
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
  /?Action=DescribeAddresses:
    get:
      summary: Describe Addresses
      description: Describes one or more of your Elastic IP addresses.
      operationId: describeaddresses
      x-api-path-slug: actiondescribeaddresses-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      - in: query
        name: PublicIp.N
        description: One or more Elastic IP addresses
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP ADdress
  /?Action=DescribeMovingAddresses:
    get:
      summary: Describe Moving Addresses
      description: Describes your Elastic IP addresses that are being moved to the
        EC2-VPC platform, or that are being restored to the EC2-Classic platform.
      operationId: describemovingaddresses
      x-api-path-slug: actiondescribemovingaddresses-get
      parameters:
      - in: query
        name: AssociationId
        description: '[EC2-VPC] The association ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
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
  /?Action=UnassignPrivateIpAddresses:
    get:
      summary: Unassign Private Ip Addresses
      description: Unassigns one or more secondary private IP addresses from a network
        interface.
      operationId: unassignprivateipaddresses
      x-api-path-slug: actionunassignprivateipaddresses-get
      parameters:
      - in: query
        name: Attribute
        description: The instance attribute
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP ADdress
  /?Action=AllocateAddress:
    get:
      summary: Allocate Address
      description: Acquires an Elastic IP address.
      operationId: allocateaddress
      x-api-path-slug: actionallocateaddress-get
      parameters:
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: AllowReassociation
        description: '[EC2-VPC] For a VPC in an EC2-Classic account, specify true
          to allow an Elastic IP address that is already associated with an instance
          or network interface to be reassociated with the specified instance or network
          interface'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: NetworkInterfaceId
        description: '[EC2-VPC] The ID of the network interface'
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary or secondary private IP address to associate
          with the Elastic IP address'
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
  /?Action=AssociateAddress:
    get:
      summary: Associate Address
      description: Associates an Elastic IP address with an instance or a network
        interface.
      operationId: associateaddress
      x-api-path-slug: actionassociateaddress-get
      parameters:
      - in: query
        name: AllocationId.N
        description: '[EC2-VPC] One or more allocation IDs'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: PublicIp.N
        description: '[EC2-Classic] One or more Elastic IP addresses'
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
  /?Action=DisassociateAddress:
    get:
      summary: Disassociate Address
      description: Disassociates an Elastic IP address from the instance or network
        interface it's associated with.
      operationId: disassociateaddress
      x-api-path-slug: actiondisassociateaddress-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - IIP Address
  /?Action=MoveAddressToVpc:
    get:
      summary: Move Address To Vpc
      description: Moves an Elastic IP address from the EC2-Classic platform to the
        EC2-VPC platform.
      operationId: moveaddresstovpc
      x-api-path-slug: actionmoveaddresstovpc-get
      parameters:
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
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