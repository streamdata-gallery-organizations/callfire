{
  "info": {
    "name": "Callfire Find calls",
    "_postman_id": "8e484a56-ab71-41bf-a870-5e9a3fea8557",
    "description": "To search for all calls sent or received by the user. Use \"id=0\" for the campaignId parameter to query for all calls sent through the POST /calls API. See [call states and results](https://developers.callfire.com/results-responses-errors.html)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "c92fd4e6-9d96-4fa1-b4ea-c0e5a5cc7c01",
          "name": "findCalls",
          "request": {
            "url": "http://www.callfire.com/v2/calls?batchId=%7B%7D&campaignId=%7B%7D&fields=%7B%7D&fromNumber=%7B%7D&id=%7B%7D&inbound=%7B%7D&intervalBegin=%7B%7D&intervalEnd=%7B%7D&label=%7B%7D&limit=%7B%7D&offset=%7B%7D&results=%7B%7D&states=%7B%7D&toNumber=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To search for all calls sent or received by the user. Use \"id=0\" for the campaignId parameter to query for all calls sent through the POST /calls API. See [call states and results](https://developers.callfire.com/results-responses-errors.html)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "238cfaa8-a548-4d45-9b1b-c8021fac7efa"
            }
          ]
        }
      ]
    }
  ]
}