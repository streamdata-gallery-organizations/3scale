{
  "info": {
    "name": "3scale Game Membership History",
    "_postman_id": "c133ba51-81bc-485f-893f-a689ea49e828",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "86972cc5-ffb2-4ae3-8a19-2a038df93efc",
      "name": "GameMembershipHistoryByHostnameGet",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/game-membership-history"
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
        "description": "Game Membership History"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "ece61b8c-dc4d-40dc-9ffc-866fe7d38b3a"
        }
      ]
    }
  ]
}