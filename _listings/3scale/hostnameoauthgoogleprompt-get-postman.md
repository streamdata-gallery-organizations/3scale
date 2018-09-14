{
  "info": {
    "name": "3scale Google Prompt",
    "_postman_id": "9dad3d9f-43e8-43c7-8012-96a8855215cb",
    "description": "This endpoint should be used by clients looking to authenticate users with the CAAP api through google.\n\nThe route requires a `client_id` query parameter and will redirect the user to the google oauth flow. Once the user has authenticated with google, caap will handle creating the user record and will redirect the user to the `redirect_uri` associated with the client who initiated the request.\n\nThe `redirect_uri` will receive `token` query parameter, which the client should use to then communicate with the api.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "59e5ce8b-89a0-499a-af8b-fca6a4f33d61",
      "name": "UnnammedEndpointGet",
      "request": {
        "url": "http://http://",
        "method": "GET",
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
          "mode": "raw"
        },
        "description": "Once a user has authorized a client to communicate on their behalf (via the `auth/authorize` endpoint), the client can use the generated token in their `x-client-bearer-token` header to retreive the user's information from this endpoint."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "620d40a5-9eec-419b-b21b-72e62a887a4c"
        }
      ]
    },
    {
      "id": "ae35b3ce-f9f1-4166-aa8f-3e2afc826832",
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
          "id": "160cb31b-b8dc-466f-bf19-08f7c4d5adc3"
        }
      ]
    },
    {
      "id": "685ab9b3-d5c8-4149-827e-04f34edfaaa3",
      "name": "AuthRolesByHostnameGet",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/auth/roles"
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
          "mode": "raw"
        },
        "description": "Current Roles"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fa9de00a-d8fb-4c2f-987d-111abdc8e9d8"
        }
      ]
    },
    {
      "id": "1db9e57c-7124-41b7-99f6-ddd698fcd0bc",
      "name": "OauthGooglePromptByHostnameGet",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/oauth/google/prompt"
          ],
          "query": [
            {
              "key": "client_id",
              "value": "%7B%7D",
              "disabled": false
            }
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
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "This endpoint should be used by clients looking to authenticate users with the CAAP api through google.\n\nThe route requires a `client_id` query parameter and will redirect the user to the google oauth flow. Once the user has authenticated with google, caap will handle creating the user record and will redirect the user to the `redirect_uri` associated with the client who initiated the request.\n\nThe `redirect_uri` will receive `token` query parameter, which the client should use to then communicate with the api."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2059c58c-d4c8-4754-8251-e5485f2ec67c"
        }
      ]
    }
  ]
}