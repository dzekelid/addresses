{
  "info": {
    "name": "Compute Engine",
    "_postman_id": "d91f9155-460f-40a2-a032-5658a0aabed9",
    "description": "Creates and runs virtual machines on Google Cloud Platform.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "address",
      "item": [
        {
          "id": "52c5a597-52b2-49e7-a84b-11537b83cdff",
          "name": "compute.addresses.aggregatedList",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "compute",
                "v1",
                "projects",
                ":project/aggregated/addresses"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an aggregated list of addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82013367-be54-43d1-afc6-4bd107124dba"
            }
          ]
        }
      ]
    }
  ]
}