{
  "info": {
    "name": "Shopify Get all customers with an address in the Brazil",
    "_postman_id": "aa9a8cc3-0690-4657-94e6-70186e16b29a",
    "description": "Get all customers with an address in the brazil.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "9e6cb3e8-9a97-4e43-9a6a-db34dd42a48c",
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
              "id": "73cde3e4-3471-4b2f-8440-88b00dd891c5"
            }
          ]
        },
        {
          "id": "113375cf-fdc4-4439-89ff-cdaa23228209",
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
              "id": "1cfa791a-0dff-4f17-9f4c-2aa8ead60f72"
            }
          ]
        },
        {
          "id": "66861c85-9b0a-46e5-b8e4-2663791db170",
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
              "id": "d73d7dc9-bfc3-4ca6-879e-f29482a7c0bd"
            }
          ]
        },
        {
          "id": "724049f2-4986-4511-b23c-d0263791d141",
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
              "id": "972ad10b-9faa-4336-b6ae-d9e257c3f045"
            }
          ]
        }
      ]
    }
  ]
}