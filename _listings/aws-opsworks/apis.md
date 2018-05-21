---
name: AWS OpsWorks
x-slug: aws-opsworks
description: AWS OpsWorks is a configuration management service that uses Chef, an
  automation platform that treats server configurations as code. OpsWorks uses Chef
  to automate how servers are configured, deployed, and managed across your Amazon
  Elastic Compute Cloud (Amazon EC2) instances or on-premises compute environments.
  OpsWorks has two offerings, AWS Opsworks for Chef Automate, and AWS OpsWorks Stacks.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
x-kinRank: "10"
x-alexaRank: ""
tags: Addresses
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/apis.md
specificationVersion: "0.14"
apis:
- name: AWS OpsWorks API Associate Elastic IP
  x-api-slug: aws-opsworks-api
  description: Associates one of the stack's registered Elastic IP addresses with
    a specified instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: ://///?Action=AssociateElasticIp
  tags: IP Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/actionassociateelasticip-get-openapi.md
- name: AWS OpsWorks API Deregister Elastic IP
  x-api-slug: aws-opsworks-api
  description: Deregisters a specified Elastic IP address.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: ://///?Action=DeregisterElasticIp
  tags: IP Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/actionderegisterelasticip-get-openapi.md
- name: AWS OpsWorks API Describes Elastic IPs
  x-api-slug: aws-opsworks-api
  description: Describes Elastic IPs
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: ://///?Action=DescribeElasticIps
  tags: IP Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/actiondescribeelasticips-get-openapi.md
- name: AWS OpsWorks API Disassociate Elastic Ip
  x-api-slug: aws-opsworks-api
  description: Disassociates an Elastic IP address from its instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: ://///?Action=DisassociateElasticIp
  tags: IP Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/actiondisassociateelasticip-get-openapi.md
- name: AWS OpsWorks API Register Elastic Ip
  x-api-slug: aws-opsworks-api
  description: Registers an Elastic IP address with a specified stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: ://///?Action=RegisterElasticIp
  tags: IP Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/actionregisterelasticip-get-openapi.md
- name: AWS OpsWorks API Update Elastic Ip
  x-api-slug: aws-opsworks-api
  description: Updates a registered Elastic IP address's name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: ://///?Action=UpdateElasticIp
  tags: IP Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/actionupdateelasticip-get-openapi.md
- name: AWS OpsWorks API
  x-api-slug: aws-opsworks-api
  description: AWS OpsWorks is a configuration management service that uses Chef,
    an automation platform that treats server configurations as code. OpsWorks uses
    Chef to automate how servers are configured, deployed, and managed across your
    Amazon Elastic Compute Cloud (Amazon EC2) instances or on-premises compute environments.
    OpsWorks has two offerings, AWS Opsworks for Chef Automate, and AWS OpsWorks Stacks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSOpsWorks.png
  humanURL: https://aws.amazon.com/opsworks/
  baseURL: :///
  tags: Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/addresses/master/_listings/aws-opsworks/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/opsworks/latest/APIReference/Welcome.html
- type: x-website
  url: https://aws.amazon.com/opsworks/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---