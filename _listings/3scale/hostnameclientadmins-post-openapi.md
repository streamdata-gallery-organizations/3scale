---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale POST client admin
  description: |-
    Allows users to add another user to the client's list of admins. It is assumed that when posting to this route that the current client (based on `x-client-auth`) is the client of which the user is adding a client admin.

    (unless the user is a system admin)
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
  //{hostname}/client-admins:
    post:
      summary: POST client admin
      description: |-
        Allows users to add another user to the client's list of admins. It is assumed that when posting to this route that the current client (based on `x-client-auth`) is the client of which the user is adding a client admin.

        (unless the user is a system admin)
      operationId: ClientAdminsByHostnamePost
      x-api-path-slug: hostnameclientadmins-post
      parameters:
      - in: formData
        name: client
      - in: path
        name: hostname
      - in: formData
        name: user
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