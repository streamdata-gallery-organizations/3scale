---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale Password Login (System Clients Only)
  description: Once a user has authorized a client to communicate on their behalf
    (via the `auth/authorize` endpoint), the client can use the generated token in
    their `x-client-bearer-token` header to retreive the user's information from this
    endpoint.
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
  //:
    get:
      summary: Current User
      description: Once a user has authorized a client to communicate on their behalf
        (via the `auth/authorize` endpoint), the client can use the generated token
        in their `x-client-bearer-token` header to retreive the user's information
        from this endpoint.
      operationId: UnnammedEndpointGet
      x-api-path-slug: get
      parameters:
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/auth/tokens:
    get:
      summary: Available Tokens
      description: In order for a given client to retreive a list of tokens that users
        have created for the client to communicate with, they can send a request (with
        the `x-client-auth` header set appropriately) to this endpoint.
      operationId: AuthTokensByHostnameGet
      x-api-path-slug: hostnameauthtokens-get
      parameters:
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/auth/roles:
    get:
      summary: Current Roles
      description: ""
      operationId: AuthRolesByHostnameGet
      x-api-path-slug: hostnameauthroles-get
      parameters:
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
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
  //{hostname}/oauth/google/auth:
    get:
      summary: Google Callback
      description: This endpoint should never be accessed directly by clients, it
        is only ever used during the google oauth process during oauth.
      operationId: OauthGoogleAuthByHostnameGet
      x-api-path-slug: hostnameoauthgoogleauth-get
      parameters:
      - in: path
        name: hostname
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/auth:
    post:
      summary: Password Login (System Clients Only)
      description: Once a user has authorized a client to communicate on their behalf
        (via the `auth/authorize` endpoint), the client can use the generated token
        in their `x-client-bearer-token` header to retreive the user's information
        from this endpoint.
      operationId: AuthByHostnamePost
      x-api-path-slug: hostnameauth-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
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