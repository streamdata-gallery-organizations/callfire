{
  "info": {
    "name": "Callfire Get call recordings for a call",
    "_postman_id": "4d5f629d-0998-49c3-a476-31bf3a424037",
    "description": "Returns a list of recordings metadata of particular call. Metadata contains link to a MP3 recording",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "3a11e8df-6bad-439b-b6cc-d01855e2347d",
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
              "id": "acfe0df3-27db-44cf-ac5a-15d01fdc0647"
            }
          ]
        },
        {
          "id": "af005aeb-ac77-46b0-916b-f0995efcfa9c",
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
              "id": "81adc584-7064-47c0-94e5-96603d052873"
            }
          ]
        },
        {
          "id": "93d099e1-7bfa-4469-a25d-be12bb28fe21",
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
              "id": "1ae8b700-8fc8-4556-b732-62b06d797709"
            }
          ]
        }
      ]
    }
  ]
}