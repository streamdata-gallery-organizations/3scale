{
  "info": {
    "name": "3scale Service Management API Authorize (App Id authentication pattern)",
    "_postman_id": "9ff7223b-8abe-472b-a1d5-c08406dbc97f",
    "description": "Authorize (app id authentication pattern).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transactions",
      "item": [
        {
          "id": "058006ba-4be0-4817-819e-39b6557bfba6",
          "name": "report",
          "request": {
            "url": "http://su1.3scale.net/transactions.xml?provider_key=%7B%7D&service_id=%7B%7D&transactions=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Report (app id authentication pattern)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57530daa-371b-43d7-bd0f-810c6a029b78"
            }
          ]
        },
        {
          "id": "9ce3295a-c0ad-4aca-8ac5-2bd6e376ac93",
          "name": "authorize",
          "request": {
            "url": "http://su1.3scale.net/transactions/authorize.xml?app_id=%7B%7D&app_key=%7B%7D&provider_key=%7B%7D&referrer=%7B%7D&service_id=%7B%7D&usage=%7B%7D&user_id=%7B%7D&user_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Authorize (app id authentication pattern)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "415f7400-f1a7-4932-a652-f10be2ed74c3"
            }
          ]
        }
      ]
    }
  ]
}