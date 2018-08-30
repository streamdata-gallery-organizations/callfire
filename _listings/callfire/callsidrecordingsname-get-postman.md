{
  "info": {
    "name": "Callfire Get call recording by name",
    "_postman_id": "bb66d5bb-3b74-4908-a86c-a17f6293c39f",
    "description": "Returns recording metadata of particular call. Metadata contains link to a MP3 recording",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "57650e62-fd50-454f-bf22-1ed536bc8057",
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
              "id": "44d96417-91b9-4962-a333-5c290e21922a"
            }
          ]
        },
        {
          "id": "7f6b6226-6d0b-4330-8aa8-82d52782915f",
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
              "id": "28efdc0d-ebd7-4018-a282-81029c0b5dde"
            }
          ]
        },
        {
          "id": "fe55b59b-559f-4c1a-bbdc-df277207fe94",
          "name": "getCallRecordings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "calls/:id/recordings"
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
            "description": "Returns a list of recordings metadata of particular call. Metadata contains link to a MP3 recording"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be31d0a1-2721-44a7-9794-1084a67792e6"
            }
          ]
        },
        {
          "id": "a00dfd0e-3bdb-40fe-a0da-9ec304bdb0e6",
          "name": "getCallRecordingByName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "calls/:id/recordings/:name"
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
                },
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns recording metadata of particular call. Metadata contains link to a MP3 recording"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71365663-fab1-46a2-8688-f01eb25d8f23"
            }
          ]
        }
      ]
    }
  ]
}