{
  "info": {
    "name": "Shopify Get a single customers address",
    "_postman_id": "ead092d4-3739-4674-a2f0-df73c6e27001",
    "description": "Get a single customers address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "e56344f5-9230-4e33-9d83-0f8a207a4a64",
          "name": "getAdminCustomers3989659651Addresses.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all of a customer's addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0dd00584-d996-491b-b758-aa3ad070002b"
            }
          ]
        },
        {
          "id": "d871957a-2ef6-40c0-b392-d3582e585ce0",
          "name": "putAdminCustomers3989659651AddressesSet.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/set.json?address_ids=%5B%7B%7D%5D&operation=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Destroying multiple customer addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d363d95b-7a10-4408-bcdc-a6894d68946e"
            }
          ]
        },
        {
          "id": "ea741523-2ba3-480b-8eaf-0a301ea8290f",
          "name": "deleteAdminCustomers3989659651Addresses5484465742.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/5484465742.json",
            "method": "DELETE",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removing a customers address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d23af6dc-1d51-4c35-98a7-aaf75fbae396"
            }
          ]
        },
        {
          "id": "184acffd-bd39-4e7b-ab46-91366178287f",
          "name": "getAdminCustomersSearch.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/search.json?query=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all customers with an address in the brazil."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdbf5392-0dda-476e-9459-338e800292ea"
            }
          ]
        },
        {
          "id": "ccd7d562-835b-4c8a-8958-5a76cb04ccf4",
          "name": "putAdminCustomers3989659651Addresses5436816654Default.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/5436816654/default.json",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Assigning a new default address to a customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cee1470e-d2bc-4073-80c9-998b3ee78a3b"
            }
          ]
        },
        {
          "id": "2fd4d835-0709-4a22-b5db-1c17201f9121",
          "name": "getAdminCustomers3989659651Addresses5436816654.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/5436816654.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a single customers address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cf91268-356f-4fe5-8d8f-db739fcf8efd"
            }
          ]
        }
      ]
    }
  ]
}