{
  "info": {
    "name": "Callfire Find webhooks",
    "_postman_id": "5a01d22d-841a-4574-93d3-c7910176af0e",
    "description": "Searches all webhooks available for a current user. Searches by name, resource, event, callback URL, or whether they are enabled. Returns a paged list of Webhooks",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "e632f943-75f9-4d91-9eb4-4879fb3a671d",
          "name": "findWebhooks",
          "request": {
            "url": "http://www.callfire.com/v2/webhooks?callback=%7B%7D&enabled=%7B%7D&event=%7B%7D&fields=%7B%7D&limit=%7B%7D&name=%7B%7D&offset=%7B%7D&resource=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches all webhooks available for a current user. Searches by name, resource, event, callback URL, or whether they are enabled. Returns a paged list of Webhooks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e35130bb-4380-4275-ae7a-105b93648ac3"
            }
          ]
        }
      ]
    }
  ]
}