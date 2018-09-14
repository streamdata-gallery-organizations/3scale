---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Signup Express
  description: Signup express.
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
  /admin/api/signup.xml:
    post:
      summary: Signup Express
      description: Signup express.
      operationId: signup
      x-api-path-slug: adminapisignup-xml-post
      parameters:
      - in: query
        name: account_plan_id
        description: id of the account plan (if not assigned default will be used
          instead)
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: query
        name: application_plan_id
        description: id of the application plan (if not assigned default will be used
          instead)
      - in: query
        name: email
        description: Email of the admin user
      - in: query
        name: org_name
        description: Organization Name of the buyer account
      - in: query
        name: password
        description: Password of the admin user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: service_plan_id
        description: id of the service plan (if not assigned default will be used
          instead)
      - in: query
        name: username
        description: Username of the admin user (on the new buyer account)
      responses:
        200:
          description: OK
      tags:
      - Signup
      - Express
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