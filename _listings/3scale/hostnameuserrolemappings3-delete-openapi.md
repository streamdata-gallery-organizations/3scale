---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale DELETE user-role-mapping  (admin only)
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
  //{hostname}/user-role-mappings/3:
    delete:
      summary: DELETE user-role-mapping  (admin only)
      description: ""
      operationId: UserRoleMappings3ByHostnameDelete
      x-api-path-slug: hostnameuserrolemappings3-delete
      parameters:
      - in: path
        name: hostname
      - in: formData
        name: role
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