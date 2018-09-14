---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Webhooks Delete Failed Deliveries
  description: Webhooks delete failed deliveries.
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/api/webhooks/failures.xml:
    delete:
      summary: Webhooks Delete Failed Deliveries
      description: Webhooks delete failed deliveries.
      operationId: webhooks
      x-api-path-slug: adminapiwebhooksfailures-xml-delete
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: time
        description: Only failed webhook deliveries whose time is less or equal than
          the passed time are destroyed (if used)
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - ""
      - Failed
      - Deliveries
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---