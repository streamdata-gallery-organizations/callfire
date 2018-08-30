{
  "info": {
    "name": "Callfire Find texts",
    "_postman_id": "c92e1f8e-acf7-47d8-b3cb-43c0e7822356",
    "description": "Searches for texts sent or received by user. Use \"campaignId=0\" parameter to query for all texts sent through the POST /texts API. See [call states and results](https://developers.callfire.com/results-responses-errors.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Texts",
      "item": [
        {
          "id": "20ba4bd2-ea6a-4ffd-afdd-aaf43d17d0ec",
          "name": "findTexts",
          "request": {
            "url": "http://www.callfire.com/v2/texts?batchId=%7B%7D&campaignId=%7B%7D&fields=%7B%7D&fromNumber=%7B%7D&id=%7B%7D&inbound=%7B%7D&intervalBegin=%7B%7D&intervalEnd=%7B%7D&label=%7B%7D&limit=%7B%7D&offset=%7B%7D&results=%7B%7D&states=%7B%7D&toNumber=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for texts sent or received by user. Use \"campaignId=0\" parameter to query for all texts sent through the POST /texts API. See [call states and results](https://developers.callfire.com/results-responses-errors.html)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "489b5e02-3cc4-44f7-9696-4c1a8cb3eed1"
            }
          ]
        }
      ]
    }
  ]
}