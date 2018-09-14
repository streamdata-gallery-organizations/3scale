---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale http://{{hostname}}/socket
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
  //{hostname}/socket/:
    get:
      summary: http://{{hostname}}/socket
      description: ""
      operationId: SocketByHostnameGet
      x-api-path-slug: hostnamesocket-get
      parameters:
      - in: header
        name: Connection
      - in: path
        name: hostname
      - in: header
        name: Sec-Websocket-Key
      - in: header
        name: Sec-Websocket-Version
      - in: header
        name: Upgrade
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