---
name: 3scale
x-slug: 3scale
description: 3scales API Management platform gives you the tools you need to take
  control of your API. Trusted by more customers than any other vendor.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
x-kinRank: "10"
x-alexaRank: "333433"
tags: 3scale
created: "2018-08-29"
modified: "2018-08-29"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apis.md
specificationVersion: "0.14"
apis:
- name: Charcoal API - Current User
  x-api-slug: get
  description: Once a user has authorized a client to communicate on their behalf
    (via the `auth/authorize` endpoint), the client can use the generated token in
    their `x-client-bearer-token` header to retreive the user's information from this
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/get-openapi.md
- name: Charcoal API - Available Tokens
  x-api-slug: hostnameauthtokens-get
  description: In order for a given client to retreive a list of tokens that users
    have created for the client to communicate with, they can send a request (with
    the `x-client-auth` header set appropriately) to this endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameauthtokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameauthtokens-get-openapi.md
- name: Charcoal API - Current Roles
  x-api-slug: hostnameauthroles-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameauthroles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameauthroles-get-openapi.md
- name: Charcoal API - Google Prompt
  x-api-slug: hostnameoauthgoogleprompt-get
  description: |-
    This endpoint should be used by clients looking to authenticate users with the CAAP api through google.

    The route requires a `client_id` query parameter and will redirect the user to the google oauth flow. Once the user has authenticated with google, caap will handle creating the user record and will redirect the user to the `redirect_uri` associated with the client who initiated the request.

    The `redirect_uri` will receive `token` query parameter, which the client should use to then communicate with the api.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameoauthgoogleprompt-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameoauthgoogleprompt-get-openapi.md
- name: Charcoal API - Google Callback
  x-api-slug: hostnameoauthgoogleauth-get
  description: This endpoint should never be accessed directly by clients, it is only
    ever used during the google oauth process during oauth.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameoauthgoogleauth-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameoauthgoogleauth-get-openapi.md
- name: Charcoal API - Password Login (System Clients Only)
  x-api-slug: hostnameauth-post
  description: Once a user has authorized a client to communicate on their behalf
    (via the `auth/authorize` endpoint), the client can use the generated token in
    their `x-client-bearer-token` header to retreive the user's information from this
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameauth-post-openapi.md
- name: Charcoal API - GET client admins
  x-api-slug: hostnameclientadmins-get
  description: |-
    This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

    Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclientadmins-get-openapi.md
- name: Charcoal API - POST client admin
  x-api-slug: hostnameclientadmins-post
  description: |-
    Allows users to add another user to the client's list of admins. It is assumed that when posting to this route that the current client (based on `x-client-auth`) is the client of which the user is adding a client admin.

    (unless the user is a system admin)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclientadmins-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclientadmins-post-openapi.md
- name: Charcoal API - DELETE client admin
  x-api-slug: hostnameclientadmins5-delete
  description: Allows users to delete a mapping from user to client that represents
    the user being a client admin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclientadmins5-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclientadmins5-delete-openapi.md
- name: Charcoal API - GET clients
  x-api-slug: hostnameclients-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclients-get-openapi.md
- name: Charcoal API - POST client
  x-api-slug: hostnameclients-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclients-post-openapi.md
- name: Charcoal API - UPDATE client
  x-api-slug: hostnameclients2-patch
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclients2-patch-openapi.md
- name: Charcoal API - GET client tokens (admin only)
  x-api-slug: hostnameclienttokens-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclienttokens-get-openapi.md
- name: Charcoal API - POST client token (admin only)
  x-api-slug: hostnameclienttokens-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameclienttokens-post-openapi.md
- name: Charcoal API - Find Games
  x-api-slug: hostnamegames-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegames-get-openapi.md
- name: Charcoal API - Create Game
  x-api-slug: hostnamegames-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegames-post-openapi.md
- name: Charcoal API - End Game
  x-api-slug: hostnamegames2-patch
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegames2-patch-openapi.md
- name: Charcoal API - Delete Game
  x-api-slug: hostnamegames3-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegames3-delete-openapi.md
- name: Charcoal API - Find Game Rounds
  x-api-slug: hostnamegamerounds-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamerounds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamerounds-get-openapi.md
- name: Charcoal API - Create Game Round
  x-api-slug: hostnamegamerounds-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamerounds-post-openapi.md
- name: Charcoal API - Update Game Round
  x-api-slug: hostnamegamerounds1-patch
  description: |-
    This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

    Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamerounds1-patch-openapi.md
- name: Charcoal API - Delete game Round
  x-api-slug: hostnamegamerounds13-delete
  description: |-
    This endpoint is used to access the user-client mappings that represent a user's ability to edit client information.

    Unless the user is a system admin, this list will be filtered by the current client in order to prevent clients from accessing other client's information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamerounds13-delete-openapi.md
- name: Charcoal API - Find Game Memberships
  x-api-slug: hostnamegamememberships-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamememberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamememberships-get-openapi.md
- name: Charcoal API - Create Game Membership
  x-api-slug: hostnamegamememberships-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamememberships-post-openapi.md
- name: Charcoal API - Update Game Membership
  x-api-slug: hostnamegamememberships4-patch
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamememberships4-patch-openapi.md
- name: Charcoal API - Delete Game Membership
  x-api-slug: hostnamegamememberships3-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamememberships3-delete-openapi.md
- name: Charcoal API - Game Membership History
  x-api-slug: hostnamegamemembershiphistory-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamemembershiphistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegamemembershiphistory-get-openapi.md
- name: Charcoal API - POST callbacks/mailgun BAD
  x-api-slug: hostnamecallbacksmailgun-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamecallbacksmailgun-post-openapi.md
- name: Charcoal API - GET photos
  x-api-slug: hostnamephotos-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamephotos-get-openapi.md
- name: Charcoal API - POST photos
  x-api-slug: hostnamephotos-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamephotos-post-openapi.md
- name: Charcoal API - DELETE photos
  x-api-slug: hostnamephotos11-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamephotos11-delete-openapi.md
- name: Charcoal API - POST photos (client-only)
  x-api-slug: local-api-caap-oiq-io8080photos-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/local-api-caap-oiq-io8080photos-post-openapi.md
- name: Charcoal API - GET photo view
  x-api-slug: hostnamephotos1view-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamephotos1view-get-openapi.md
- name: Charcoal API - http://{{hostname}}/socket
  x-api-slug: hostnamesocket-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamesocket-get-openapi.md
- name: Charcoal API - GET system
  x-api-slug: hostnamesystem-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamesystem-get-openapi.md
- name: Charcoal API - UPDATE system  (admin only)
  x-api-slug: hostnamesystem-patch
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamesystem-patch-openapi.md
- name: Charcoal API - GET system email domains (admin only)
  x-api-slug: hostnamesystemdomains-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamesystemdomains-get-openapi.md
- name: Charcoal API - POST  system email domain (admin only)
  x-api-slug: hostnamesystemdomains-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamesystemdomains-post-openapi.md
- name: Charcoal API - DELETE  system email domain (admin only)
  x-api-slug: hostnamesystemdomains2-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamesystemdomains2-delete-openapi.md
- name: Charcoal API - GET activity
  x-api-slug: hostnameactivity-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameactivity-get-openapi.md
- name: Charcoal API - GET display-schedules
  x-api-slug: hostnamedisplayschedules-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamedisplayschedules-get-openapi.md
- name: Charcoal API - PATCH display-schedule
  x-api-slug: hostnamedisplayschedules1-patch
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamedisplayschedules1-patch-openapi.md
- name: Charcoal API - GET feed
  x-api-slug: hostnameactivitylive-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameactivitylive-get-openapi.md
- name: Charcoal API - GET users
  x-api-slug: hostnameusers-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameusers-get-openapi.md
- name: Charcoal API - POST users
  x-api-slug: hostnameusers-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameusers-post-openapi.md
- name: Charcoal API - PATCH users
  x-api-slug: hostnameusers1-patch
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameusers1-patch-openapi.md
- name: Charcoal API - GET user roles
  x-api-slug: hostnameuserroles-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameuserroles-get-openapi.md
- name: Charcoal API - GET google-accounts
  x-api-slug: hostnamegoogleaccounts-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnamegoogleaccounts-get-openapi.md
- name: Charcoal API - GET user-role-mappings
  x-api-slug: hostnameuserrolemappings-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameuserrolemappings-get-openapi.md
- name: Charcoal API - POST user-role-mappings  (admin only)
  x-api-slug: hostnameuserrolemappings-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameuserrolemappings-post-openapi.md
- name: Charcoal API - DELETE user-role-mapping  (admin only)
  x-api-slug: hostnameuserrolemappings3-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://http://
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/hostnameuserrolemappings3-delete-openapi.md
- name: 3Scale Account Management API - Account List
  x-api-slug: adminapiaccounts-xml-get
  description: Account list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccounts-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccounts-xml-get-openapi.md
- name: 3Scale Account Management API - Account Find
  x-api-slug: adminapiaccountsfind-xml-get
  description: Account find.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsfind-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsfind-xml-get-openapi.md
- name: 3Scale Account Management API - Application List
  x-api-slug: adminapiaccountsaccount-idapplications-xml-get
  description: Application list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-get-openapi.md
- name: 3Scale Account Management API - Application Create
  x-api-slug: adminapiaccountsaccount-idapplications-xml-post
  description: Application create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-post-openapi.md
- name: 3Scale Account Management API - Application Key List
  x-api-slug: adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-get
  description: Application key list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-get-openapi.md
- name: 3Scale Account Management API - Application key Create
  x-api-slug: adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-post
  description: Application key create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-post-openapi.md
- name: 3Scale Account Management API - Application key Delete
  x-api-slug: adminapiaccountsaccount-idapplicationsapplication-idkeyskey-xml-delete
  description: Application key delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeyskey-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeyskey-xml-delete-openapi.md
- name: 3Scale Account Management API - Application Referrer Filter List
  x-api-slug: adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-get
  description: Application referrer filter list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-get-openapi.md
- name: 3Scale Account Management API - Application referrer filter Create
  x-api-slug: adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-post
  description: Application referrer filter create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-post-openapi.md
- name: 3Scale Account Management API - Application referrer filter Delete
  x-api-slug: adminapiaccountsaccount-idapplicationsapplication-idreferrer-filtersid-xml-delete
  description: Application referrer filter delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filtersid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filtersid-xml-delete-openapi.md
- name: 3Scale Account Management API - Application Read
  x-api-slug: adminapiaccountsaccount-idapplicationsid-xml-get
  description: Application read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-get-openapi.md
- name: 3Scale Account Management API - Application Update
  x-api-slug: adminapiaccountsaccount-idapplicationsid-xml-put
  description: Application update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-put-openapi.md
- name: 3Scale Account Management API - Application Accept
  x-api-slug: adminapiaccountsaccount-idapplicationsidaccept-xml-put
  description: Application accept.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidaccept-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidaccept-xml-put-openapi.md
- name: 3Scale Account Management API - Application Change Plan
  x-api-slug: adminapiaccountsaccount-idapplicationsidchange-plan-xml-put
  description: Application change plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidchange-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidchange-plan-xml-put-openapi.md
- name: 3Scale Account Management API - Application Create Plan Customization
  x-api-slug: adminapiaccountsaccount-idapplicationsidcustomize-plan-xml-put
  description: Application create plan customization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidcustomize-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidcustomize-plan-xml-put-openapi.md
- name: 3Scale Account Management API - Application Delete Plan Customization
  x-api-slug: adminapiaccountsaccount-idapplicationsiddecustomize-plan-xml-put
  description: Application delete plan customization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsiddecustomize-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsiddecustomize-plan-xml-put-openapi.md
- name: 3Scale Account Management API - Application Resume
  x-api-slug: adminapiaccountsaccount-idapplicationsidresume-xml-put
  description: Application resume.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidresume-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidresume-xml-put-openapi.md
- name: 3Scale Account Management API - Application Suspend
  x-api-slug: adminapiaccountsaccount-idapplicationsidsuspend-xml-put
  description: Application suspend.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidsuspend-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidsuspend-xml-put-openapi.md
- name: 3Scale Account Management API - Account Message
  x-api-slug: adminapiaccountsaccount-idmessages-xml-post
  description: Account message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idmessages-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idmessages-xml-post-openapi.md
- name: 3Scale Account Management API - Account Fetch Account Plan
  x-api-slug: adminapiaccountsaccount-idplan-xml-get
  description: Account fetch account plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idplan-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idplan-xml-get-openapi.md
- name: 3Scale Account Management API - User List
  x-api-slug: adminapiaccountsaccount-idusers-xml-get
  description: User list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-get-openapi.md
- name: 3Scale Account Management API - User Create
  x-api-slug: adminapiaccountsaccount-idusers-xml-post
  description: User create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-post-openapi.md
- name: 3Scale Account Management API - User Delete
  x-api-slug: adminapiaccountsaccount-idusersid-xml-delete
  description: User delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-delete-openapi.md
- name: 3Scale Account Management API - User Read
  x-api-slug: adminapiaccountsaccount-idusersid-xml-get
  description: User read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-get-openapi.md
- name: 3Scale Account Management API - User Update
  x-api-slug: adminapiaccountsaccount-idusersid-xml-put
  description: User update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-put-openapi.md
- name: 3Scale Account Management API - User Activate
  x-api-slug: adminapiaccountsaccount-idusersidactivate-xml-put
  description: User activate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidactivate-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidactivate-xml-put-openapi.md
- name: 3Scale Account Management API - User change Role to Admin
  x-api-slug: adminapiaccountsaccount-idusersidadmin-xml-put
  description: User change role to admin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidadmin-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidadmin-xml-put-openapi.md
- name: 3Scale Account Management API - User change Role to Member
  x-api-slug: adminapiaccountsaccount-idusersidmember-xml-put
  description: User change role to member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidmember-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidmember-xml-put-openapi.md
- name: 3Scale Account Management API - User Suspend
  x-api-slug: adminapiaccountsaccount-idusersidsuspend-xml-put
  description: User suspend.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidsuspend-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidsuspend-xml-put-openapi.md
- name: 3Scale Account Management API - User Unsuspend
  x-api-slug: adminapiaccountsaccount-idusersidunsuspend-xml-put
  description: User unsuspend.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidunsuspend-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidunsuspend-xml-put-openapi.md
- name: 3Scale Account Management API - Account Delete
  x-api-slug: adminapiaccountsid-xml-delete
  description: Account delete .
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-delete-openapi.md
- name: 3Scale Account Management API - Account Read
  x-api-slug: adminapiaccountsid-xml-get
  description: Account read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-get-openapi.md
- name: 3Scale Account Management API - Account Update
  x-api-slug: adminapiaccountsid-xml-put
  description: Account update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-put-openapi.md
- name: 3Scale Account Management API - Account Approve
  x-api-slug: adminapiaccountsidapprove-xml-put
  description: Account approve.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidapprove-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidapprove-xml-put-openapi.md
- name: 3Scale Account Management API - Account Change Plan
  x-api-slug: adminapiaccountsidchange-plan-xml-put
  description: Account change plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidchange-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidchange-plan-xml-put-openapi.md
- name: 3Scale Account Management API - Account Delete Credit Card
  x-api-slug: adminapiaccountsidcredit-card-xml-delete
  description: Account delete credit card.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-delete-openapi.md
- name: 3Scale Account Management API - Account Set Credit Card
  x-api-slug: adminapiaccountsidcredit-card-xml-put
  description: Account set credit card.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-put-openapi.md
- name: 3Scale Account Management API - Account Reset to Pending
  x-api-slug: adminapiaccountsidmake-pending-xml-put
  description: Account reset to pending.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidmake-pending-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidmake-pending-xml-put-openapi.md
- name: 3Scale Account Management API - Account Reject
  x-api-slug: adminapiaccountsidreject-xml-put
  description: Account reject.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidreject-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidreject-xml-put-openapi.md
- name: 3Scale Account Management API - Account Plan List
  x-api-slug: adminapiaccount-plans-xml-get
  description: Account plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-get-openapi.md
- name: 3Scale Account Management API - Account Plan Create
  x-api-slug: adminapiaccount-plans-xml-post
  description: Account plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-post-openapi.md
- name: 3Scale Account Management API - Account Plan Feature List
  x-api-slug: adminapiaccount-plansaccount-plan-idfeatures-xml-get
  description: Account plan feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeatures-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API - Account Plan Features Delete
  x-api-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete
  description: Account plan features delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API - Account Plan Features Create
  x-api-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-post
  description: Account plan features create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-post-openapi.md
- name: 3Scale Account Management API - Account Plan Delete
  x-api-slug: adminapiaccount-plansid-xml-delete
  description: Account plan delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-delete-openapi.md
- name: 3Scale Account Management API - Account Plan Read
  x-api-slug: adminapiaccount-plansid-xml-get
  description: Account plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-get-openapi.md
- name: 3Scale Account Management API - Account Plan Update
  x-api-slug: adminapiaccount-plansid-xml-put
  description: Account plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-put-openapi.md
- name: 3Scale Account Management API - Account Plan set to Default
  x-api-slug: adminapiaccount-plansiddefault-xml-put
  description: Account plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansiddefault-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API - ActiveDocs JSON Spec Update
  x-api-slug: adminapiactive-docsid-xml-put
  description: Activedocs json spec update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiactive-docsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiactive-docsid-xml-put-openapi.md
- name: 3Scale Account Management API - Application List (all services)
  x-api-slug: adminapiapplications-xml-get
  description: Application list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplications-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplications-xml-get-openapi.md
- name: 3Scale Account Management API - Application Find
  x-api-slug: adminapiapplicationsfind-xml-get
  description: Application find.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplicationsfind-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplicationsfind-xml-get-openapi.md
- name: 3Scale Account Management API - Application Plan List (all services)
  x-api-slug: adminapiapplication-plans-xml-get
  description: Application plan list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plans-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plans-xml-get-openapi.md
- name: 3Scale Account Management API - Application Plan Feature List
  x-api-slug: adminapiapplication-plansapplication-plan-idfeatures-xml-get
  description: Application plan feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API - Application Plan Feature Create
  x-api-slug: adminapiapplication-plansapplication-plan-idfeatures-xml-post
  description: Application plan feature create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-post-openapi.md
- name: 3Scale Account Management API - Application Plan Feature Delete
  x-api-slug: adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete
  description: Application plan feature delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API - Limits List per Application Plan
  x-api-slug: adminapiapplication-plansapplication-plan-idlimits-xml-get
  description: Limits list per application plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idlimits-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idlimits-xml-get-openapi.md
- name: 3Scale Account Management API - Limit List per Metric
  x-api-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-get
  description: Limit list per metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-get-openapi.md
- name: 3Scale Account Management API - Limit Create
  x-api-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-post
  description: Limit create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-post-openapi.md
- name: 3Scale Account Management API - Limit Delete
  x-api-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-delete
  description: Limit delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-delete-openapi.md
- name: 3Scale Account Management API - Limit Read
  x-api-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-get
  description: Limit read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-get-openapi.md
- name: 3Scale Account Management API - Limit Update
  x-api-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-put
  description: Limit update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-put-openapi.md
- name: 3Scale Account Management API - Pricing Rules List per Metric
  x-api-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idpricing-rules-xml-get
  description: Pricing rules list per metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idpricing-rules-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idpricing-rules-xml-get-openapi.md
- name: 3Scale Account Management API - Pricing Rules List per Application Plan
  x-api-slug: adminapiapplication-plansapplication-plan-idpricing-rules-xml-get
  description: Pricing rules list per application plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idpricing-rules-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idpricing-rules-xml-get-openapi.md
- name: 3Scale Account Management API - End User Plan List (all services)
  x-api-slug: adminapiend-user-plans-xml-get
  description: End user plan list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plans-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plans-xml-get-openapi.md
- name: 3Scale Account Management API - Limit List for End User Plans
  x-api-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get
  description: Limit list for end user plans .
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get-openapi.md
- name: 3Scale Account Management API - Limit Create for End User Plans
  x-api-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-post
  description: Limit create for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-post-openapi.md
- name: 3Scale Account Management API - Limit Delete for End User Plans
  x-api-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete
  description: Limit delete for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete-openapi.md
- name: 3Scale Account Management API - Limit Read for End User Plans
  x-api-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-get
  description: Limit read for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-get-openapi.md
- name: 3Scale Account Management API - Limit Update for End User Plans
  x-api-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put
  description: Limit update for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put-openapi.md
- name: 3Scale Account Management API - Account Feature List
  x-api-slug: adminapifeatures-xml-get
  description: Account feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-get-openapi.md
- name: 3Scale Account Management API - Account Feature Create
  x-api-slug: adminapifeatures-xml-post
  description: Account feature create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-post-openapi.md
- name: 3Scale Account Management API - Account Feature Delete
  x-api-slug: adminapifeaturesid-xml-delete
  description: Account feature delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API - Account Feature Read
  x-api-slug: adminapifeaturesid-xml-get
  description: Account feature read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-get-openapi.md
- name: 3Scale Account Management API - Account Feature Update
  x-api-slug: adminapifeaturesid-xml-put
  description: Account feature update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-put-openapi.md
- name: 3Scale Account Management API - Nginx configuration files
  x-api-slug: adminapinginx-zip-get
  description: Nginx configuration files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapinginx-zip-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapinginx-zip-get-openapi.md
- name: 3Scale Account Management API - Account Read
  x-api-slug: adminapiprovider-xml-get
  description: Account read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiprovider-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiprovider-xml-get-openapi.md
- name: 3Scale Account Management API - Service List
  x-api-slug: adminapiservices-xml-get
  description: Service list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservices-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservices-xml-get-openapi.md
- name: 3Scale Account Management API - Service Create
  x-api-slug: adminapiservices-xml-post
  description: Service create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservices-xml-post-openapi.md
- name: 3Scale Account Management API - Service Read
  x-api-slug: adminapiservicesid-xml-get
  description: Service read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesid-xml-get-openapi.md
- name: 3Scale Account Management API - Service Update
  x-api-slug: adminapiservicesid-xml-put
  description: Service update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesid-xml-put-openapi.md
- name: 3Scale Account Management API - Service Plan List
  x-api-slug: adminapiservicesidservice-plans-xml-get
  description: Service plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesidservice-plans-xml-get-openapi.md
- name: 3Scale Account Management API - Service Plan Create
  x-api-slug: adminapiservicesidservice-plans-xml-post
  description: Service plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesidservice-plans-xml-post-openapi.md
- name: 3Scale Account Management API - Application Plan List
  x-api-slug: adminapiservicesservice-idapplication-plans-xml-get
  description: Application plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plans-xml-get-openapi.md
- name: 3Scale Account Management API - Application Plan Create
  x-api-slug: adminapiservicesservice-idapplication-plans-xml-post
  description: Application plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plans-xml-post-openapi.md
- name: 3Scale Account Management API - Application Plan Delete
  x-api-slug: adminapiservicesservice-idapplication-plansid-xml-delete
  description: Application plan delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansid-xml-delete-openapi.md
- name: 3Scale Account Management API - Application Plan Read
  x-api-slug: adminapiservicesservice-idapplication-plansid-xml-get
  description: Application plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansid-xml-get-openapi.md
- name: 3Scale Account Management API - Application Plan Update
  x-api-slug: adminapiservicesservice-idapplication-plansid-xml-put
  description: Application plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansid-xml-put-openapi.md
- name: 3Scale Account Management API - Application Plan set to Default
  x-api-slug: adminapiservicesservice-idapplication-plansiddefault-xml-put
  description: Application plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API - End User Create
  x-api-slug: adminapiservicesservice-idend-users-xml-post
  description: End user create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-users-xml-post-openapi.md
- name: 3Scale Account Management API - End User Delete
  x-api-slug: adminapiservicesservice-idend-usersusername-xml-delete
  description: End user delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-usersusername-xml-delete-openapi.md
- name: 3Scale Account Management API - End User Read
  x-api-slug: adminapiservicesservice-idend-usersusername-xml-get
  description: End user read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-usersusername-xml-get-openapi.md
- name: 3Scale Account Management API - End User Change Plan
  x-api-slug: adminapiservicesservice-idend-usersusernamechange-plan-xml-put
  description: End user change plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-usersusernamechange-plan-xml-put-openapi.md
- name: 3Scale Account Management API - End User Plan List
  x-api-slug: adminapiservicesservice-idend-user-plans-xml-get
  description: End user plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plans-xml-get-openapi.md
- name: 3Scale Account Management API - End User Plan Create
  x-api-slug: adminapiservicesservice-idend-user-plans-xml-post
  description: End user plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plans-xml-post-openapi.md
- name: 3Scale Account Management API - End User Plan Read
  x-api-slug: adminapiservicesservice-idend-user-plansid-xml-get
  description: End user plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plansid-xml-get-openapi.md
- name: 3Scale Account Management API - End User Plan Update
  x-api-slug: adminapiservicesservice-idend-user-plansid-xml-put
  description: End user plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plansid-xml-put-openapi.md
- name: 3Scale Account Management API - End User Plan set to Default
  x-api-slug: adminapiservicesservice-idend-user-plansiddefault-xml-put
  description: End user plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API - Service Feature List
  x-api-slug: adminapiservicesservice-idfeatures-xml-get
  description: Service feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API - Service Feature Create
  x-api-slug: adminapiservicesservice-idfeatures-xml-post
  description: Service feature create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeatures-xml-post-openapi.md
- name: 3Scale Account Management API - Service Feature Delete
  x-api-slug: adminapiservicesservice-idfeaturesid-xml-delete
  description: Service feature delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API - Service Feature Read
  x-api-slug: adminapiservicesservice-idfeaturesid-xml-get
  description: Service feature read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeaturesid-xml-get-openapi.md
- name: 3Scale Account Management API - Service Feature Update
  x-api-slug: adminapiservicesservice-idfeaturesid-xml-put
  description: Service feature update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeaturesid-xml-put-openapi.md
- name: 3Scale Account Management API - Metric List
  x-api-slug: adminapiservicesservice-idmetrics-xml-get
  description: Metric list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetrics-xml-get-openapi.md
- name: 3Scale Account Management API - Metric Create
  x-api-slug: adminapiservicesservice-idmetrics-xml-post
  description: Metric create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetrics-xml-post-openapi.md
- name: 3Scale Account Management API - Metric Delete
  x-api-slug: adminapiservicesservice-idmetricsid-xml-delete
  description: Metric delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsid-xml-delete-openapi.md
- name: 3Scale Account Management API - Metric Read
  x-api-slug: adminapiservicesservice-idmetricsid-xml-get
  description: Metric read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsid-xml-get-openapi.md
- name: 3Scale Account Management API - Metric Update
  x-api-slug: adminapiservicesservice-idmetricsid-xml-put
  description: Metric update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsid-xml-put-openapi.md
- name: 3Scale Account Management API - Method List
  x-api-slug: adminapiservicesservice-idmetricsmetric-idmethods-xml-get
  description: Method list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethods-xml-get-openapi.md
- name: 3Scale Account Management API - Method Create
  x-api-slug: adminapiservicesservice-idmetricsmetric-idmethods-xml-post
  description: Method create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethods-xml-post-openapi.md
- name: 3Scale Account Management API - Method Delete
  x-api-slug: adminapiservicesservice-idmetricsmetric-idmethodsid-xml-delete
  description: Method delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethodsid-xml-delete-openapi.md
- name: 3Scale Account Management API - Method Read
  x-api-slug: adminapiservicesservice-idmetricsmetric-idmethodsid-xml-get
  description: Method read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethodsid-xml-get-openapi.md
- name: 3Scale Account Management API - Method Update
  x-api-slug: adminapiservicesservice-idmetricsmetric-idmethodsid-xml-put
  description: Method update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethodsid-xml-put-openapi.md
- name: 3Scale Account Management API - Service Plan Delete
  x-api-slug: adminapiservicesservice-idservice-plansid-xml-delete
  description: Service plan delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansid-xml-delete-openapi.md
- name: 3Scale Account Management API - Service Plan Read
  x-api-slug: adminapiservicesservice-idservice-plansid-xml-get
  description: Service plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansid-xml-get-openapi.md
- name: 3Scale Account Management API - Service Plan Update
  x-api-slug: adminapiservicesservice-idservice-plansid-xml-put
  description: Service plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansid-xml-put-openapi.md
- name: 3Scale Account Management API - Service Plan set to Default
  x-api-slug: adminapiservicesservice-idservice-plansiddefault-xml-put
  description: Service plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API - Service Plan List (all services)
  x-api-slug: adminapiservice-plans-xml-get
  description: Service plan list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservice-plans-xml-get-openapi.md
- name: 3Scale Account Management API - Service Plan Feature List
  x-api-slug: adminapiservice-plansservice-plan-idfeatures-xml-get
  description: Service plan feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservice-plansservice-plan-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API - Service Plan Feature Add
  x-api-slug: adminapiservice-plansservice-plan-idfeatures-xml-post
  description: Service plan feature add.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservice-plansservice-plan-idfeatures-xml-post-openapi.md
- name: 3Scale Account Management API - Signup Express
  x-api-slug: adminapisignup-xml-post
  description: Signup express.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapisignup-xml-post-openapi.md
- name: 3Scale Account Management API - User List (provider account)
  x-api-slug: adminapiusers-xml-get
  description: User list (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusers-xml-get-openapi.md
- name: 3Scale Account Management API - User Create (provider account)
  x-api-slug: adminapiusers-xml-post
  description: User create (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusers-xml-post-openapi.md
- name: 3Scale Account Management API - User Delete (provider account)
  x-api-slug: adminapiusersid-xml-delete
  description: User delete (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersid-xml-delete-openapi.md
- name: 3Scale Account Management API - User Read (provider account)
  x-api-slug: adminapiusersid-xml-get
  description: User read (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersid-xml-get-openapi.md
- name: 3Scale Account Management API - User Update (provider account)
  x-api-slug: adminapiusersid-xml-put
  description: User update (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersid-xml-put-openapi.md
- name: 3Scale Account Management API - User Activate (provider account)
  x-api-slug: adminapiusersidactivate-xml-put
  description: User activate (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidactivate-xml-put-openapi.md
- name: 3Scale Account Management API - User change Role to Admin (provider account)
  x-api-slug: adminapiusersidadmin-xml-put
  description: User change role to admin (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidadmin-xml-put-openapi.md
- name: 3Scale Account Management API - User change Role to Member (provider account)
  x-api-slug: adminapiusersidmember-xml-put
  description: User change role to member (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidmember-xml-put-openapi.md
- name: 3Scale Account Management API - User Suspend (provider account)
  x-api-slug: adminapiusersidsuspend-xml-put
  description: User suspend (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidsuspend-xml-put-openapi.md
- name: 3Scale Account Management API - User Unsuspend (of provider account)
  x-api-slug: adminapiusersidunsuspend-xml-put
  description: User unsuspend (of provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidunsuspend-xml-put-openapi.md
- name: 3Scale Account Management API - Webhooks Delete Failed Deliveries
  x-api-slug: adminapiwebhooksfailures-xml-delete
  description: Webhooks delete failed deliveries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiwebhooksfailures-xml-delete-openapi.md
- name: 3Scale Account Management API - Webhooks List Failed Deliveries
  x-api-slug: adminapiwebhooksfailures-xml-get
  description: Webhooks list failed deliveries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiwebhooksfailures-xml-get-openapi.md
- name: 3Scale Analytics API - Application Usage by Metric
  x-api-slug: statsapplicationsapplication-idusage-format-get
  description: Application usage by metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsapplicationsapplication-idusage-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsapplicationsapplication-idusage-format-get-openapi.md
- name: 3Scale Analytics API - Service Top Applications
  x-api-slug: statsservicesservice-idtop-applications-format-get
  description: Service top applications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idtop-applications-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idtop-applications-format-get-openapi.md
- name: 3Scale Analytics API - Service Usage by Metric
  x-api-slug: statsservicesservice-idusage-format-get
  description: Service usage by metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idusage-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idusage-format-get-openapi.md
- name: 3Scale Billing API - Invoice List by Account
  x-api-slug: apiaccountsaccount-idinvoices-xml-get
  description: Invoice list by account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoices-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoices-xml-get-openapi.md
- name: 3Scale Billing API - Invoice by Account
  x-api-slug: apiaccountsaccount-idinvoicesid-xml-get
  description: Invoice by account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoicesid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoicesid-xml-get-openapi.md
- name: 3Scale Billing API - Invoice List
  x-api-slug: apiinvoices-xml-get
  description: Invoice list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoices-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoices-xml-get-openapi.md
- name: 3Scale Billing API - Invoice
  x-api-slug: apiinvoicesid-xml-get
  description: Invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesid-xml-get-openapi.md
- name: 3Scale Billing API - Invoice
  x-api-slug: apiinvoicesidstate-xml-put
  description: Invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesidstate-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesidstate-xml-put-openapi.md
- name: 3Scale Billing API - Invoice Line Items List
  x-api-slug: apiinvoicesinvoice-idline-items-xml-get
  description: Invoice line items list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idline-items-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idline-items-xml-get-openapi.md
- name: 3Scale Billing API - Invoice Payment Transactions List
  x-api-slug: apiinvoicesinvoice-idpayment-transactions-xml-get
  description: Invoice payment transactions list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idpayment-transactions-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idpayment-transactions-xml-get-openapi.md
- name: 3scale Service Management API - Report (App Id authentication pattern)
  x-api-slug: transactions-xml-post
  description: Report (app id authentication pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactions-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactions-xml-post-openapi.md
- name: 3scale Service Management API - Authorize (App Id authentication pattern)
  x-api-slug: transactionsauthorize-xml-get
  description: Authorize (app id authentication pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthorize-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthorize-xml-get-openapi.md
- name: 3scale Service Management API - AuthRep (Authorize + Report for the App Id
    authentication pattern)
  x-api-slug: transactionsauthrep-xml-get
  description: Authrep (authorize + report for the app id authentication pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthrep-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthrep-xml-get-openapi.md
- name: 3scale Service Management API - Authorize (Oauth authentication mode pattern)
  x-api-slug: transactionsoauth-authorize-xml-get
  description: Authorize (oauth authentication mode pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Management, Management, My API Stack, Imports, Stack Network, SaaS, Technology,
    Enterprise, API Service Provider, Profiles, Portals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsoauth-authorize-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsoauth-authorize-xml-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://3scale.api.gallery.streamdata.io
- type: x-api-stack
  url: http://3scale.stack.network
- type: x-blog
  url: http://www.3scale.net/blog/
- type: x-blog-rss
  url: http://www.3scale.net/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/3scale
- type: x-crunchbase
  url: https://crunchbase.com/organization/3scale
- type: x-email
  url: sales@3scale.net
- type: x-email
  url: info@3scale.net
- type: x-github
  url: https://github.com/3scale
- type: x-pricing
  url: https://www.3scale.net/pricing/
- type: x-privacy
  url: https://www.3scale.net/privacy-policy/
- type: x-support
  url: https://support.3scale.net
- type: x-openapi-spec
  url: https://support.3scale.net/reference/active-docs
- type: x-terms-of-service
  url: https://www.3scale.net/terms-and-conditions/
- type: x-twitter
  url: https://twitter.com/3scale
- type: x-website
  url: http://3scale.net
- type: x-website
  url: http://
- type: x-website
  url: http://http
- type: x-website
  url: http://www.3scale.net
- type: x-website
  url: ://
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---