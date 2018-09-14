---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Service Feature Update
  description: Service feature update.
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
  /admin/api/services/{service_id}/features/{id}.xml:
    put:
      summary: Service Feature Update
      description: Service feature update.
      operationId: service_feature
      x-api-path-slug: adminapiservicesservice-idfeaturesid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: name
        description: Name of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Service
      - Feature
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