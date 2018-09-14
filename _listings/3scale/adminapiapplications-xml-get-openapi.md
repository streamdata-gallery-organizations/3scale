---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Application List (all services)
  description: Application list (all services).
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
  /admin/api/applications.xml:
    get:
      summary: Application List (all services)
      description: Application list (all services).
      operationId: application
      x-api-path-slug: adminapiapplications-xml-get
      parameters:
      - in: query
        name: active_since
        description: filter date
      - in: query
        name: inactive_since
        description: filter date
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: service_id
        description: filter by service
      responses:
        200:
          description: OK
      tags:
      - Application
      - List
      - (all
      - Services)
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