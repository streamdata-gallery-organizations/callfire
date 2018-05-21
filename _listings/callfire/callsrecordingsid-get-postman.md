{
  "info": {
    "name": "Callfire Get call recording by id",
    "_postman_id": "5a1c63be-6c64-4bf9-8515-9211a55467c7",
    "description": "Returns metadata of recording of a particular call. Metadata contains a link to a MP3 recording",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "9c34ba9f-326a-4a1e-9925-8fcbd627d0ce",
          "name": "getCallRecording",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "calls/recordings/:id"
              ],
              "query": [
                {
                  "key": "fields",
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
            "description": "Returns metadata of recording of a particular call. Metadata contains a link to a MP3 recording"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa8fc4e0-b576-4593-8cae-3009cd3c311a"
            }
          ]
        }
      ]
    }
  ]
}