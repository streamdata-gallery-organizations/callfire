{
  "info": {
    "name": "Callfire Download media by extension",
    "_postman_id": "ee345c9a-0994-4437-b32a-2b725e06e811",
    "description": "Download a media file. Available types of files: bmp, gif, jpg, m4a, mp3, mp4, png, wav. Content type in response depends on 'extension' parameter, e.g. image/jpeg, image/png, audio/mp3, etc",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Media",
      "item": [
        {
          "id": "fd87a603-c39b-43fb-8f61-90401adb31be",
          "name": "getMediaDataByKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "media/public/:key.:extension"
              ],
              "variable": [
                {
                  "id": "extension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download a media file. Available types of files: bmp, gif, jpg, m4a, mp3, mp4, png, wav. Content type in response depends on 'extension' parameter, e.g. image/jpeg, image/png, audio/mp3, etc"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b8c6e0e-3c70-4a2d-a956-8b4d67bc3318"
            }
          ]
        }
      ]
    }
  ]
}