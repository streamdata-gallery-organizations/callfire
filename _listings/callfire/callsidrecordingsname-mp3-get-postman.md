{
  "info": {
    "name": "Callfire Get call mp3 recording by name",
    "_postman_id": "aa52b6ac-81b2-46e4-8be9-56d62061e55c",
    "description": "Returns a MP3 recording of a particular call, response contains binary data, content type is 'audio/mpeg'",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "b2d0cdd7-a296-4a52-8483-a9b0a78d1c75",
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
              "id": "31008986-028b-45d5-a2a3-d2234ba98c9a"
            }
          ]
        },
        {
          "id": "ac3bebdf-64ac-47b8-a5a9-e842e247e39a",
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
              "id": "740f819e-1db7-4d88-b7fa-d7341b081dbc"
            }
          ]
        },
        {
          "id": "668bbe08-5503-4297-9827-73d007cf9c6b",
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
              "id": "6586c8be-0170-419b-8816-fad6f34f9b4b"
            }
          ]
        },
        {
          "id": "c096e9f9-064f-4023-9da9-04443df43d7b",
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
              "id": "f44eaeac-c8cf-4f6f-ba04-52b96ad21460"
            }
          ]
        },
        {
          "id": "401265ff-ffe4-4493-bc24-995891c360b5",
          "name": "getCallRecordingMp3ByName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "calls/:id/recordings/:name.mp3"
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
            "description": "Returns a MP3 recording of a particular call, response contains binary data, content type is 'audio/mpeg'"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "741e9092-4e66-40c5-b67b-7606039d31ac"
            }
          ]
        }
      ]
    }
  ]
}