---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale POST  system email domain (admin only)
  description: ""
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
  //{hostname}/client-admins:
    get:
      summary: GET client admins
      description: |-
        This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

        Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
      operationId: ClientAdminsByHostnameGet
      x-api-path-slug: hostnameclientadmins-get
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
    post:
      summary: POST client admin
      description: |-
        Allows users to add another user to the client's list of admins. It is assumed that when posting to this route that the current client (based on `x-client-auth`) is the client of which the user is adding a client admin.

        (unless the user is a system admin)
      operationId: ClientAdminsByHostnamePost
      x-api-path-slug: hostnameclientadmins-post
      parameters:
      - in: formData
        name: client
      - in: path
        name: hostname
      - in: formData
        name: user
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/client-admins/5:
    delete:
      summary: DELETE client admin
      description: Allows users to delete a mapping from user to client that represents
        the user being a client admin.
      operationId: ClientAdmins5ByHostnameDelete
      x-api-path-slug: hostnameclientadmins5-delete
      parameters:
      - in: path
        name: hostname
      - in: formData
        name: user
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/clients:
    get:
      summary: GET clients
      description: ""
      operationId: ClientsByHostnameGet
      x-api-path-slug: hostnameclients-get
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
    post:
      summary: POST client
      description: ""
      operationId: ClientsByHostnamePost
      x-api-path-slug: hostnameclients-post
      parameters:
      - in: formData
        name: description
      - in: path
        name: hostname
      - in: formData
        name: name
      - in: formData
        name: redirect_uri
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/clients/2:
    patch:
      summary: UPDATE client
      description: ""
      operationId: Clients2ByHostnamePatch
      x-api-path-slug: hostnameclients2-patch
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
  //{hostname}/client-tokens:
    get:
      summary: GET client tokens (admin only)
      description: ""
      operationId: ClientTokensByHostnameGet
      x-api-path-slug: hostnameclienttokens-get
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
    post:
      summary: POST client token (admin only)
      description: ""
      operationId: ClientTokensByHostnamePost
      x-api-path-slug: hostnameclienttokens-post
      parameters:
      - in: formData
        name: client
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
  //{hostname}/games:
    get:
      summary: Find Games
      description: ""
      operationId: GamesByHostnameGet
      x-api-path-slug: hostnamegames-get
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
    post:
      summary: Create Game
      description: ""
      operationId: GamesByHostnamePost
      x-api-path-slug: hostnamegames-post
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
  //{hostname}/games/2:
    patch:
      summary: End Game
      description: ""
      operationId: Games2ByHostnamePatch2
      x-api-path-slug: hostnamegames2-patch
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
  //{hostname}/games/3:
    delete:
      summary: Delete Game
      description: ""
      operationId: Games3ByHostnameDelete
      x-api-path-slug: hostnamegames3-delete
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
  //{hostname}/game-rounds:
    get:
      summary: Find Game Rounds
      description: ""
      operationId: GameRoundsByHostnameGet
      x-api-path-slug: hostnamegamerounds-get
      parameters:
      - in: query
        name: filter[game_id]
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
    post:
      summary: Create Game Round
      description: ""
      operationId: GameRoundsByHostnamePost
      x-api-path-slug: hostnamegamerounds-post
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
  //{hostname}/game-rounds/1:
    patch:
      summary: Update Game Round
      description: |-
        This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

        Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
      operationId: GameRounds1ByHostnamePatch
      x-api-path-slug: hostnamegamerounds1-patch
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
  //{hostname}/game-rounds/13:
    delete:
      summary: Delete game Round
      description: |-
        This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

        Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
      operationId: GameRounds13ByHostnameDelete
      x-api-path-slug: hostnamegamerounds13-delete
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
  //{hostname}/game-memberships:
    get:
      summary: Find Game Memberships
      description: ""
      operationId: GameMembershipsByHostnameGet
      x-api-path-slug: hostnamegamememberships-get
      parameters:
      - in: query
        name: filter[game_id]
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
    post:
      summary: Create Game Membership
      description: ""
      operationId: GameMembershipsByHostnamePost
      x-api-path-slug: hostnamegamememberships-post
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
  //{hostname}/game-memberships/4:
    patch:
      summary: Update Game Membership
      description: ""
      operationId: GameMemberships4ByHostnamePatch
      x-api-path-slug: hostnamegamememberships4-patch
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
  //{hostname}/game-memberships/3:
    delete:
      summary: Delete Game Membership
      description: ""
      operationId: GameMemberships3ByHostnameDelete
      x-api-path-slug: hostnamegamememberships3-delete
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
  //{hostname}/game-membership-history:
    get:
      summary: Game Membership History
      description: ""
      operationId: GameMembershipHistoryByHostnameGet
      x-api-path-slug: hostnamegamemembershiphistory-get
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
  //{hostname}/callbacks/mailgun:
    post:
      summary: POST callbacks/mailgun BAD
      description: ""
      operationId: CallbacksMailgunByHostnamePost4
      x-api-path-slug: hostnamecallbacksmailgun-post
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: hostname
      - in: formData
        name: message-url
      - in: query
        name: secret
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/photos:
    get:
      summary: GET photos
      description: ""
      operationId: PhotosByHostnameGet
      x-api-path-slug: hostnamephotos-get
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
    post:
      summary: POST photos
      description: ""
      operationId: PhotosByHostnamePost
      x-api-path-slug: hostnamephotos-post
      parameters:
      - in: path
        name: hostname
      - in: formData
        name: label
      - in: formData
        name: photo
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/photos/11:
    delete:
      summary: DELETE photos
      description: ""
      operationId: Photos11ByHostnameDelete
      x-api-path-slug: hostnamephotos11-delete
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
  //local.api.caap.oiq.io:8080/photos:
    post:
      summary: POST photos (client-only)
      description: ""
      operationId: LocalApiCaapOiqIo8080PhotosPost
      x-api-path-slug: local-api-caap-oiq-io8080photos-post
      parameters:
      - in: formData
        name: label
      - in: formData
        name: photo
      - in: header
        name: x-client-auth
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/photos/1/view:
    get:
      summary: GET photo view
      description: ""
      operationId: Photos1ViewByHostnameGet
      x-api-path-slug: hostnamephotos1view-get
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
  //{hostname}/socket/:
    get:
      summary: http://{{hostname}}/socket
      description: ""
      operationId: SocketByHostnameGet
      x-api-path-slug: hostnamesocket-get
      parameters:
      - in: header
        name: Connection
      - in: path
        name: hostname
      - in: header
        name: Sec-Websocket-Key
      - in: header
        name: Sec-Websocket-Version
      - in: header
        name: Upgrade
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/system:
    get:
      summary: GET system
      description: ""
      operationId: SystemByHostnameGet
      x-api-path-slug: hostnamesystem-get
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
    patch:
      summary: UPDATE system  (admin only)
      description: ""
      operationId: SystemByHostnamePatch
      x-api-path-slug: hostnamesystem-patch
      parameters:
      - in: path
        name: hostname
      - in: formData
        name: restricted_email_domains
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/system/domains:
    get:
      summary: GET system email domains (admin only)
      description: ""
      operationId: SystemDomainsByHostnameGet
      x-api-path-slug: hostnamesystemdomains-get
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
    post:
      summary: POST  system email domain (admin only)
      description: ""
      operationId: SystemDomainsByHostnamePost
      x-api-path-slug: hostnamesystemdomains-post
      parameters:
      - in: formData
        name: domain
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