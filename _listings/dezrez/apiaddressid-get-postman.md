{
  "info": {
    "name": "Dezrez Get an address by its Id",
    "_postman_id": "40c6a88f-0569-4580-959d-0142fce6bdbf",
    "description": "Get an address by its id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Searchproperties",
      "item": [
        {
          "id": "ac4adbbd-aed1-4efb-8a9b-b44acb3e23d2",
          "name": "Property_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumberBydataContract.s",
          "request": {
            "url": "http://api.dezrez.com/api/property/suggest?dataContract.pageNumber=%7B%7D&dataContract.pageSize=%7B%7D&dataContract.query=%7B%7D&dataContract.suggestType=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Search for properties/addresses that match the specified search criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "990d8311-e93d-4e70-8681-c6427d7e5156"
            }
          ]
        }
      ]
    },
    {
      "name": "Address",
      "item": [
        {
          "id": "7ef7e3ea-5065-4839-945a-366aebe956b7",
          "name": "Address_GetByid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/address/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Get an address by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2aa192bc-254f-4682-b17c-ebe6902dcd59"
            }
          ]
        }
      ]
    }
  ]
}