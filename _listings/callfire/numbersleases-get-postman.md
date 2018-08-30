{
  "info": {
    "name": "Callfire Find leases",
    "_postman_id": "70098f64-517d-44f4-9130-479e5d6aa630",
    "description": "Searches for all numbers leased by account user. This API is useful for finding all numbers currently owned by the user. Returns a paged list of number leases.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Numbers",
      "item": [
        {
          "id": "5b316824-af2e-4765-91ec-4275e438a67f",
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
              "id": "5d130bc0-0b5c-4b15-8902-87d1da0df20c"
            }
          ]
        }
      ]
    }
  ]
}