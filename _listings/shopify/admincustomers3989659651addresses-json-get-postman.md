{
  "info": {
    "name": "Shopify Get all of a customer's addresses",
    "_postman_id": "dc4c429a-6ccf-42a0-8109-d3e9e6be3dde",
    "description": "Get all of a customer's addresses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "4b024912-6b48-4e24-8d72-2566ce575e64",
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
              "id": "f4777a36-57d0-4264-b318-4f0fde745c62"
            }
          ]
        }
      ]
    }
  ]
}