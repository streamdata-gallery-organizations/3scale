---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Application Plan Feature Delete
  description: Application plan feature delete.
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
  /admin/api/application_plans/{application_plan_id}/features/{id}.xml:
    delete:
      summary: Application Plan Feature Delete
      description: Application plan feature delete.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
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