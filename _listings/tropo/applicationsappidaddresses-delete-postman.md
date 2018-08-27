{
  "info": {
    "name": "Tropo Delete Applications Appid Addresses",
    "_postman_id": "7705bf03-1add-4c22-9011-097b79eba8ea",
    "description": "Delete applications appid addresses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "ea9ef35f-6977-41de-9ed5-a96eb94286b1",
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
              "id": "b66d834d-2320-49c1-a61c-fef46f05030e"
            }
          ]
        }
      ]
    }
  ]
}