{
  "info": {
    "name": "Callfire Find keyword leases",
    "_postman_id": "0a9c1188-6de0-47af-8e5d-d36844620de8",
    "description": "Searches for all keywords owned by user. A keyword lease is the ownership information involving a keyword",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Keywords",
      "item": [
        {
          "id": "c612f8d1-ad16-4f68-a11b-c4a3cf4c16d4",
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
              "id": "0fd8cecb-5dfd-4175-93d2-576f36dff4c4"
            }
          ]
        },
        {
          "id": "cac45a44-72bc-4aa3-8493-24f5a3b9911f",
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
              "id": "14377349-0cb5-4377-bb4e-140ce44fa01b"
            }
          ]
        }
      ]
    }
  ]
}