{
  "info": {
    "name": "3scale Available Tokens",
    "_postman_id": "b6d5c0f5-f33b-4ccd-93f3-d0df3d2b8814",
    "description": "In order for a given client to retreive a list of tokens that users have created for the client to communicate with, they can send a request (with the `x-client-auth` header set appropriately) to this endpoint.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "7af7d7ef-bec0-428e-8a1b-6bdc7ba7406c",
      "name": "AuthTokensByHostnameGet",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/auth/tokens"
          ],
          "variable": [
            {
              "id": "hostname",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "x-client-auth",
            "value": "{}",
            "description": "",
            "disabled": false
          },
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "In order for a given client to retreive a list of tokens that users have created for the client to communicate with, they can send a request (with the `x-client-auth` header set appropriately) to this endpoint."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7b934c2a-14a6-44d3-9792-1a2c046a57ad"
        }
      ]
    }
  ]
}