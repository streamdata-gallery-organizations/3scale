{
  "info": {
    "name": "3scale Service Management API AuthRep (Authorize + Report for the App Id authentication pattern)",
    "_postman_id": "7d70f4d4-5793-4efd-9af9-817fea41de4e",
    "description": "Authrep (authorize + report for the app id authentication pattern).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transactions",
      "item": [
        {
          "id": "700dcbe1-d1ec-475c-a3e0-29f42973cd24",
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
              "id": "5f06f494-d28a-4728-9ebf-031c90e642f4"
            }
          ]
        },
        {
          "id": "0582746b-36b6-4d4f-97fd-1e100122f465",
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
              "id": "897be158-fe21-4ebe-9eb8-c6a8848b73b4"
            }
          ]
        },
        {
          "id": "750172a4-5637-4613-8992-09f0d4ad2d4f",
          "name": "authrep",
          "request": {
            "url": "http://su1.3scale.net/transactions/authrep.xml?app_id=%7B%7D&app_key=%7B%7D&log=%7B%7D&provider_key=%7B%7D&referrer=%7B%7D&service_id=%7B%7D&usage=%7B%7D&user_id=%7B%7D&user_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Authrep (authorize + report for the app id authentication pattern)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f002f321-a2da-41c4-a06d-4f7e0409c1d6"
            }
          ]
        }
      ]
    }
  ]
}