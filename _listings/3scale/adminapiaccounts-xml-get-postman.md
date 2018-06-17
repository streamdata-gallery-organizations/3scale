{
  "info": {
    "name": "3Scale Account Management API Account List",
    "_postman_id": "4bfe06ce-52dc-4688-9150-087d70851ddc",
    "description": "Account list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "68f866ef-ece2-47a5-8134-85910f213f6a",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts.xml?page=%7B%7D&per_page=%7B%7D&provider_key=%7B%7D&state=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ef3b119-5639-4763-ae0c-88443917d878"
            }
          ]
        }
      ]
    }
  ]
}