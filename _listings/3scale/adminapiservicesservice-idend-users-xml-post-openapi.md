---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API End User Create
  description: End user create.
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
  /admin/api/services/{service_id}/end_users.xml:
    post:
      summary: End User Create
      description: End user create.
      operationId: end_user
      x-api-path-slug: adminapiservicesservice-idend-users-xml-post
      parameters:
      - in: query
        name: plan_id
        description: id of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: query
        name: username
        description: username (unique identifier) of the end user
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Create
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