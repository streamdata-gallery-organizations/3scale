---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API User Create (provider account)
  description: User create (provider account).
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
  /admin/api/users.xml:
    post:
      summary: User Create (provider account)
      description: User create (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusers-xml-post
      parameters:
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: query
        name: email
        description: Email of the user
      - in: query
        name: password
        description: Password of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: username
        description: Username of the user
      responses:
        200:
          description: OK
      tags:
      - User
      - (provider
      - Account)
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