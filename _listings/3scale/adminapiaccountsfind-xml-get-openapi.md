---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Account Find
  description: Account find.
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
  /admin/api/accounts/find.xml:
    get:
      summary: Account Find
      description: Account find.
      operationId: account
      x-api-path-slug: adminapiaccountsfind-xml-get
      parameters:
      - in: query
        name: email
        description: email of the user of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: username
        description: username of the user of the account
      - in: query
        name: user_id
        description: id of the user of the account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Find
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