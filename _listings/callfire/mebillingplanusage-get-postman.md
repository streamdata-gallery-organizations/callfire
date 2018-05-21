{
  "info": {
    "name": "Callfire Find plan usage",
    "_postman_id": "bf0ce0c6-ddd6-4303-bc9c-810cac52c6ad",
    "description": "Searches for the data of a billing plan usage for the user. Returns the data of a billing plan usage for the current month",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Me",
      "item": [
        {
          "id": "4069decb-a920-455d-bd19-331a91f3cbe5",
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
              "id": "a79429a5-2d30-4f03-b7ac-0136510444ba"
            }
          ]
        },
        {
          "id": "f3909e17-1331-4267-bca3-b01711efd4fe",
          "name": "getBillingPlanUsage",
          "request": {
            "url": "http://www.callfire.com/v2/me/billing/plan-usage",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for the data of a billing plan usage for the user. Returns the data of a billing plan usage for the current month"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45d720ca-7db1-4a83-b8d8-b8eae23d83fa"
            }
          ]
        }
      ]
    }
  ]
}