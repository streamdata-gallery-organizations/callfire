{
  "info": {
    "name": "Callfire Find a specific lease",
    "_postman_id": "bef78061-b79a-4ceb-81c6-6d567fddf577",
    "description": "Searches for all keywords owned by user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Keywords",
      "item": [
        {
          "id": "0af1d166-b720-479b-a0c2-23dac9b528b3",
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
              "id": "f235dcbf-70bf-4d1d-ad23-2e1827bed8e7"
            }
          ]
        },
        {
          "id": "2eb55ff6-8310-47bf-9a54-b0145e7ab35f",
          "name": "findKeywordLeases",
          "request": {
            "url": "http://www.callfire.com/v2/keywords/leases?fields=%7B%7D&limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all keywords owned by user. A keyword lease is the ownership information involving a keyword"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ba1acdf-3cf9-4827-a1d1-0d7b4e4284a7"
            }
          ]
        },
        {
          "id": "d7c539ae-77f0-45b8-8d96-63cc6d57b711",
          "name": "getKeywordLease",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "keywords/leases/:keyword"
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
                  "id": "keyword",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all keywords owned by user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d183cd2d-6d5f-4355-b2c5-64875b353cf5"
            }
          ]
        }
      ]
    }
  ]
}