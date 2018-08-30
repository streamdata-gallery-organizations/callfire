{
  "info": {
    "name": "Callfire Find credit usage",
    "_postman_id": "b0084f35-1faf-4835-b4f1-f331a7f30bec",
    "description": "Find credit usage for the user. Returns credits usage for time period specified or if unspecified then total for all time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Me",
      "item": [
        {
          "id": "9dc050bc-fe92-4396-a146-dfa32a85d42d",
          "name": "getCreditUsage",
          "request": {
            "url": "http://www.callfire.com/v2/me/billing/credit-usage?intervalBegin=%7B%7D&intervalEnd=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Find credit usage for the user. Returns credits usage for time period specified or if unspecified then total for all time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e570eb3-3e74-4a73-99c4-caa87def5fbd"
            }
          ]
        }
      ]
    }
  ]
}