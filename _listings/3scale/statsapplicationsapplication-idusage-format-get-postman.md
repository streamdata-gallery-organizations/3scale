{
  "info": {
    "name": "3Scale Analytics API Application Usage by Metric",
    "_postman_id": "5fb3316e-912d-47cb-8fff-fc65440d98fd",
    "description": "Application usage by metric.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Application",
      "item": [
        {
          "id": "5651564f-1d0f-4d42-aca4-4fc045f8b1e9",
          "name": "application_ops",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "stats/applications/:application_id/usage.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "granularity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "metric_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_change",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "timezone",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "until",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application usage by metric."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b40e7cf-d3dc-4efe-929a-06aec5c82634"
            }
          ]
        }
      ]
    }
  ]
}