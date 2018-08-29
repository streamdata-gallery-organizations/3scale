{
  "info": {
    "name": "3scale Service Management API Report (App Id authentication pattern)",
    "_postman_id": "48f374b5-b51b-4dc8-b6fc-e620690a62e9",
    "description": "Report (app id authentication pattern).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transactions",
      "item": [
        {
          "id": "defc05e8-7e00-4a82-acf7-61ce42599584",
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
              "id": "f6082150-e9a1-4ead-be04-95d3840de8f6"
            }
          ]
        }
      ]
    }
  ]
}