---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale Google Prompt
  description: |-
    This endpoint should be used by clients looking to authenticate users with the CAAP api through google.

    The route requires a `client_id` query parameter and will redirect the user to the google oauth flow. Once the user has authenticated with google, caap will handle creating the user record and will redirect the user to the `redirect_uri` associated with the client who initiated the request.

    The `redirect_uri` will receive `token` query parameter, which the client should use to then communicate with the api.
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
  //{hostname}/oauth/google/prompt:
    get:
      summary: Google Prompt
      description: |-
        This endpoint should be used by clients looking to authenticate users with the CAAP api through google.

        The route requires a `client_id` query parameter and will redirect the user to the google oauth flow. Once the user has authenticated with google, caap will handle creating the user record and will redirect the user to the `redirect_uri` associated with the client who initiated the request.

        The `redirect_uri` will receive `token` query parameter, which the client should use to then communicate with the api.
      operationId: OauthGooglePromptByHostnameGet
      x-api-path-slug: hostnameoauthgoogleprompt-get
      parameters:
      - in: query
        name: client_id
      - in: path
        name: hostname
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