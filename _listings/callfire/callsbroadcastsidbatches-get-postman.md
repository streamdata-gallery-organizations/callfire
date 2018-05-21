{
  "info": {
    "name": "Callfire Find batches in a call broadcast",
    "_postman_id": "1e3e1ec4-58e7-487d-a14f-87a4199a14d2",
    "description": "This endpoint will enable the user to page through all of the batches for a particular voice broadcast campaign",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "f9d5bbda-281b-4807-a55b-03d4b5580c01",
          "name": "getCallBroadcastBatches",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "calls/broadcasts/:id/batches"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint will enable the user to page through all of the batches for a particular voice broadcast campaign"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36e8ae4f-2ab0-426e-98f5-edb27b666a8e"
            }
          ]
        }
      ]
    }
  ]
}