{
  "info": {
    "name": "Callfire Get call recording in mp3 format",
    "_postman_id": "93ab0f30-1544-4926-a7f3-a3d4f4156429",
    "description": "Returns an MP3 recording of particular call, response contains binary data, content type is 'audio/mpeg'",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "f8f4ea05-75e6-419e-be08-c24d78855645",
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
              "id": "0831d1ec-8881-4a01-bfe3-b1a54e29e032"
            }
          ]
        },
        {
          "id": "c17da36f-a4c7-4603-af1d-729989ee7d5d",
          "name": "getCallRecordingMp3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "calls/recordings/:id.mp3"
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
            "description": "Returns an MP3 recording of particular call, response contains binary data, content type is 'audio/mpeg'"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "685c16e3-08a8-4780-9e06-6dd130149a1a"
            }
          ]
        }
      ]
    }
  ]
}