{
  "info": {
    "name": "3scale DELETE client admin",
    "_postman_id": "8a5fdab8-61be-4a8b-8fa5-2b4f534ed808",
    "description": "Allows users to delete a mapping from user to client that represents the user being a client admin.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "ebda9b9c-6113-4ed4-9e76-775b930fc3b7",
      "name": "ClientAdminsByHostnamePost",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/client-admins"
          ],
          "variable": [
            {
              "id": "hostname",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "POST",
        "header": [
          {
            "key": "x-client-auth",
            "value": "{}",
            "description": "",
            "disabled": false
          },
          {
            "key": "x-client-bearer-token",
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
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "client",
              "value": "{}",
              "disabled": false,
              "description": ""
            },
            {
              "key": "user",
              "value": "{}",
              "disabled": false,
              "description": ""
            }
          ]
        },
        "description": "Allows users to add another user to the client's list of admins. It is assumed that when posting to this route that the current client (based on `x-client-auth`) is the client of which the user is adding a client admin.\n\n(unless the user is a system admin)"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "aa67de3f-3538-4cdf-9fb8-7fba967f0de9"
        }
      ]
    },
    {
      "id": "6447e0ad-600c-4abc-9437-264244c1d44e",
      "name": "ClientAdmins5ByHostnameDelete",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/client-admins/5"
          ],
          "variable": [
            {
              "id": "hostname",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "DELETE",
        "header": [
          {
            "key": "x-client-auth",
            "value": "{}",
            "description": "",
            "disabled": false
          },
          {
            "key": "x-client-bearer-token",
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
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "user",
              "value": "{}",
              "disabled": false,
              "description": ""
            }
          ]
        },
        "description": "Allows users to delete a mapping from user to client that represents the user being a client admin."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e1ecc416-b4c7-4a05-8955-4bf37f19e7f3"
        }
      ]
    }
  ]
}