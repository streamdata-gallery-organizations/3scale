---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale Delete game Round
  description: |-
    This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

    Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
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
  //{hostname}/game-rounds/13:
    delete:
      summary: Delete game Round
      description: |-
        This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

        Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
      operationId: GameRounds13ByHostnameDelete
      x-api-path-slug: hostnamegamerounds13-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
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