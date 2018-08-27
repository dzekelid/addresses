{
  "info": {
    "name": "AWS EC2 API Unassign Ipv6 Addresses",
    "_postman_id": "e1dcc722-6fa3-48d6-8513-8bb9f56c0325",
    "description": "Unassigns one or more IPv6 addresses from a network interface.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IPv6 Addresses",
      "item": [
        {
          "id": "6ed85385-5587-4850-a91b-5675843d20b8",
          "name": "unassignipv6addresses",
          "request": {
            "url": "http://example.com/api/?Action=UnassignIpv6Addresses?NetworkInterfaceId=NetworkInterfaceId&PrivateIpAddress.N=PrivateIpAddress.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unassigns one or more IPv6 addresses from a network interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9d435b2-e02a-4d69-8b20-9f0edfc09bf0"
            }
          ]
        }
      ]
    }
  ]
}