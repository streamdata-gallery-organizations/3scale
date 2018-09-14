---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Method Create
  description: Method create.
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
  /admin/api/services/{service_id}/metrics/{metric_id}/methods.xml:
    post:
      summary: Method Create
      description: Method create.
      operationId: metric_method
      x-api-path-slug: adminapiservicesservice-idmetricsmetric-idmethods-xml-post
      parameters:
      - in: query
        name: friendly_name
        description: Name of the method
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: query
        name: system_name
        description: System Name of the metric
      - in: query
        name: unit
        description: Measure unit of the method
      responses:
        200:
          description: OK
      tags:
      - Method
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