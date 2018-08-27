{
  "info": {
    "name": "Shopify Removing a customers address",
    "_postman_id": "89e8267e-33c5-4542-92ee-ce9b75a9f933",
    "description": "Removing a customers address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "f28677f6-6773-476e-b32b-93896836f7f3",
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
              "id": "a30668a3-68f5-4a8f-af32-871e0319b805"
            }
          ]
        },
        {
          "id": "0906dbc5-3aca-4c22-9271-4dc63217441f",
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
              "id": "f8060eb6-4b82-438e-83ba-ba0e7cff60a1"
            }
          ]
        },
        {
          "id": "754bf6c2-2279-496e-b0c0-8522f4e8ed48",
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
              "id": "72db4d2b-7026-484c-818e-ac18cf1cd62b"
            }
          ]
        }
      ]
    }
  ]
}