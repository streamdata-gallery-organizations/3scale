---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale Available Tokens
  description: In order for a given client to retreive a list of tokens that users
    have created for the client to communicate with, they can send a request (with
    the `x-client-auth` header set appropriately) to this endpoint.
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
  //{hostname}/auth/tokens:
    get:
      summary: Available Tokens
      description: In order for a given client to retreive a list of tokens that users
        have created for the client to communicate with, they can send a request (with
        the `x-client-auth` header set appropriately) to this endpoint.
      operationId: AuthTokensByHostnameGet
      x-api-path-slug: hostnameauthtokens-get
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