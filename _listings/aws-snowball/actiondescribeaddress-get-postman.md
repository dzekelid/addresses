{
  "info": {
    "name": "AWS Snowball API Describe Address",
    "_postman_id": "3e6f3d29-4de3-4f00-b3bb-4991d2030412",
    "description": "Takes an AddressId and returns specific details about that address in the\n      form of an Address object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Addresses",
      "item": [
        {
          "id": "f2634b0c-eee3-400f-b33a-f7cb11bdeb29",
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
              "id": "9b75ebad-c16c-447f-81b6-adf883aac64b"
            }
          ]
        },
        {
          "id": "51551d9d-5563-4f02-828f-7ea47e3ab7a9",
          "name": "describeAddress",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAddress?AddressId=AddressId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Takes an AddressId and returns specific details about that address in the\n      form of an Address object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5067aca3-b723-4b9c-9c21-6861f24a58c0"
            }
          ]
        }
      ]
    }
  ]
}