---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale POST photos (client-only)
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
  //local.api.caap.oiq.io:8080/photos:
    post:
      summary: POST photos (client-only)
      description: ""
      operationId: LocalApiCaapOiqIo8080PhotosPost
      x-api-path-slug: local-api-caap-oiq-io8080photos-post
      parameters:
      - in: formData
        name: label
      - in: formData
        name: photo
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