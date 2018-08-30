{
  "info": {
    "name": "Callfire Find lease configs",
    "_postman_id": "b0791229-8e99-498d-b361-22ddf833fcfd",
    "description": "Searches for all number lease configs for the user. Returns a paged list of NumberConfig",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Numbers",
      "item": [
        {
          "id": "f49ca371-310c-46b5-8eaa-36c2c6aca61f",
          "name": "findNumberLeases",
          "request": {
            "url": "http://www.callfire.com/v2/numbers/leases?city=%7B%7D&fields=%7B%7D&labelName=%7B%7D&lata=%7B%7D&limit=%7B%7D&offset=%7B%7D&prefix=%7B%7D&rateCenter=%7B%7D&state=%7B%7D&zipcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all numbers leased by account user. This API is useful for finding all numbers currently owned by the user. Returns a paged list of number leases."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65da822d-e6e9-45a4-a562-2a231e3ab51a"
            }
          ]
        },
        {
          "id": "bd09d1f8-5dc5-49fb-93e2-d3296bb79818",
          "name": "findNumberLeaseConfigs",
          "request": {
            "url": "http://www.callfire.com/v2/numbers/leases/configs?city=%7B%7D&fields=%7B%7D&labelName=%7B%7D&lata=%7B%7D&limit=%7B%7D&offset=%7B%7D&prefix=%7B%7D&rateCenter=%7B%7D&state=%7B%7D&zipcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all number lease configs for the user. Returns a paged list of NumberConfig"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a061cf13-68e8-4f21-9fd9-b992f0bc045e"
            }
          ]
        }
      ]
    }
  ]
}