{
  "info": {
    "name": "3scale POST client admin",
    "_postman_id": "cbe7c4e7-376c-463d-ad69-99979548ab04",
    "description": "Allows users to add another user to the client's list of admins. It is assumed that when posting to this route that the current client (based on `x-client-auth`) is the client of which the user is adding a client admin.\n\n(unless the user is a system admin)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "73f7f774-869f-462c-8033-82e98a1b6622",
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
          "id": "a238e6ab-5a2d-4d48-9f94-372d7358f395"
        }
      ]
    },
    {
      "id": "e292c954-732a-4504-a908-a4636066e048",
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
          "id": "33641349-c2ee-40d6-8332-01fc7ba04d1a"
        }
      ]
    }
  ]
}