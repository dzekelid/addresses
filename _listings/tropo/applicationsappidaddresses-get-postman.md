{
  "info": {
    "name": "Tropo Get Applications Appid Addresses",
    "_postman_id": "84a73412-36b3-453d-9b8d-8f03a19f139e",
    "description": "Get applications appid addresses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "0e9b4bcc-c9f4-4f36-9c43-8877404940e3",
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
              "id": "e45dabd6-0bba-4762-a286-4b25ee8e04bc"
            }
          ]
        },
        {
          "id": "8d1ec72b-8ced-4b31-b06b-3c69d4874cbb",
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
              "id": "c197fab4-c78a-43e5-b52c-512cd388c824"
            }
          ]
        }
      ]
    }
  ]
}