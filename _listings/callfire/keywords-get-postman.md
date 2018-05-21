{
  "info": {
    "name": "Callfire Find keywords",
    "_postman_id": "37aacfeb-9037-4b90-ae54-fb0290a52c86",
    "description": "Searches for all keywords available for purchase on the CallFire platform. If a keyword appears in the response, it is available for purchase. List the 'keywords' in a query parameter to search for multiple keywords (at least one keyword should be sent in request)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Keywords",
      "item": [
        {
          "id": "279585af-ece7-40bc-858a-6cb2b0408bd4",
          "name": "findKeywords",
          "request": {
            "url": "http://www.callfire.com/v2/keywords?keywords=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all keywords available for purchase on the CallFire platform. If a keyword appears in the response, it is available for purchase. List the 'keywords' in a query parameter to search for multiple keywords (at least one keyword should be sent in request)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "386f8746-5d0b-44b3-bec1-901d3ad4785b"
            }
          ]
        }
      ]
    }
  ]
}