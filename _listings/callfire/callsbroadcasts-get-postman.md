{
  "info": {
    "name": "Callfire Find call broadcasts",
    "_postman_id": "15dcc502-ff05-4980-b533-762a6dd83030",
    "description": "Searches for all voice broadcasts created by user. Can query on label, name, and the current running status of the campaign. Returns a paged list of voice broadcasts",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "4245c1b4-1997-4c1d-b8d0-63caab5be30a",
          "name": "findCallBroadcasts",
          "request": {
            "url": "http://www.callfire.com/v2/calls/broadcasts?fields=%7B%7D&label=%7B%7D&limit=%7B%7D&name=%7B%7D&offset=%7B%7D&running=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all voice broadcasts created by user. Can query on label, name, and the current running status of the campaign. Returns a paged list of voice broadcasts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51df8b5e-3488-4f16-aad8-81ab59c40c26"
            }
          ]
        }
      ]
    }
  ]
}