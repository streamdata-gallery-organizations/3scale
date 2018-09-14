---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Analytics API Application Usage by Metric
  description: Application usage by metric.
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
  /stats/applications/{application_id}/usage.{format}:
    get:
      summary: Application Usage by Metric
      description: Application usage by metric.
      operationId: application_ops
      x-api-path-slug: statsapplicationsapplication-idusage-format-get
      parameters:
      - in: path
        name: application_id
        description: id of the application
      - in: path
        name: format
        description: Response format
      - in: query
        name: granularity
        description: Granularity of the results
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
      - in: query
        name: since
        description: Time range start
      - in: query
        name: skip_change
        description: Skip period over period calculations (setting this to true will
          increase the performance of the call)
      - in: query
        name: timezone
        description: Timezone to do the calculations in
      - in: query
        name: until
        description: Time range end
      responses:
        200:
          description: OK
      tags:
      - Application
      - Usage
      - By
      - Metric
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