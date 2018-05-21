{
  "info": {
    "name": "AWS Snowball API Create Address",
    "_postman_id": "82a4579f-96ad-4aa1-aeec-68ee4c4b1170",
    "description": "Creates an address for a Snowball to be shipped to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Addresses",
      "item": [
        {
          "id": "b8d485a5-6ecd-4c75-ad26-65ba020fbb07",
          "name": "createAddress",
          "request": {
            "url": "http://example.com/api/?Action=CreateAddress?Address=Address",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an address for a Snowball to be shipped to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06395a4c-7ebd-4c0f-86b1-a71d5d0de0a7"
            }
          ]
        }
      ]
    }
  ]
}