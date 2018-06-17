{
  "info": {
    "name": "3Scale Account Management API Application List",
    "_postman_id": "76c6d194-308c-434f-a7c4-4a170a246080",
    "description": "Application list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "8410be33-6c1b-40e9-bdc7-3bc67482d856",
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
              "id": "f2956e02-effc-4877-90ab-efbe4f056217"
            }
          ]
        },
        {
          "id": "870f49d2-8f73-47ae-ae1f-19c28859fa54",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts/find.xml?email=%7B%7D&provider_key=%7B%7D&username=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account find."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "208c04d8-2835-40f7-a4b3-7f779bb38363"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "9493ffeb-e577-495d-83d4-1388cd9bd1cf",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "770b25ef-5cc6-4470-9604-4958ef17e782"
            }
          ]
        }
      ]
    }
  ]
}