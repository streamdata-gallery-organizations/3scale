---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Analytics API Service Top Applications
  description: Service top applications.
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
  /stats/services/{service_id}/top_applications.{format}:
    get:
      summary: Service Top Applications
      description: Service top applications.
      operationId: service_ops
      x-api-path-slug: statsservicesservice-idtop-applications-format-get
      parameters:
      - in: path
        name: format
        description: Response format
      - in: query
        name: metric_name
        description: System name of metric for which to get data
      - in: query
        name: period
        description: 'Period, combined with since give the stats for the time range
          [since '
      - in: query
        name: provider_key
        description: Your api key with 3scale
      - in: path
        name: service_id
        description: id of the service
      - in: query
        name: since
        description: Time range start
      responses:
        200:
          description: OK
      tags:
      - Service
      - Top
      - Applications
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