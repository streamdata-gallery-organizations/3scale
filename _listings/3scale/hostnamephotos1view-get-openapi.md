---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale GET photo view
  description: ""
  version: "1.0"
host: 'http:'
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  //{hostname}/photos/1/view:
    get:
      summary: GET photo view
      description: ""
      operationId: Photos1ViewByHostnameGet
      x-api-path-slug: hostnamephotos1view-get
      parameters:
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      responses:
        200:
          description: OK
      tags:
      - ""
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