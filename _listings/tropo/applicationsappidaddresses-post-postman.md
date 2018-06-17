{
  "info": {
    "name": "Tropo Post Applications Appid Addresses",
    "_postman_id": "c59f3981-6409-4cd0-89de-95f8ebc93879",
    "description": "Post applications appid addresses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "318f6a01-fd86-40b7-8779-b246310dc30e",
          "name": "getApplicationsAppAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tropo.com",
              "path": [
                "v1",
                "applications/:AppId/addresses"
              ],
              "query": [
                {
                  "key": "applicationId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AppId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get applications appid addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04890daa-0364-4a00-8ce6-f86d87217bce"
            }
          ]
        },
        {
          "id": "f47ad1b4-1459-49fc-9a00-dea9c56a18bb",
          "name": "postApplicationsAppAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tropo.com",
              "path": [
                "v1",
                "applications/:AppId/addresses"
              ],
              "query": [
                {
                  "key": "applicationId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AppId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post applications appid addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33e5e6e0-ec0d-4f97-9451-8600b47aee15"
            }
          ]
        },
        {
          "id": "65678c58-7d6d-439c-a5b7-60d4b6dbfad2",
          "name": "deleteApplicationsAppAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tropo.com",
              "path": [
                "v1",
                "applications/:AppId/addresses"
              ],
              "query": [
                {
                  "key": "applicationId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AppId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete applications appid addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d02f68d-c6b7-4f30-9f76-95c799080bee"
            }
          ]
        }
      ]
    }
  ]
}