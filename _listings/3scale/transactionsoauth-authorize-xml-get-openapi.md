---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale Service Management API Authorize (Oauth authentication mode pattern)
  description: Authorize (oauth authentication mode pattern).
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
  /transactions.xml:
    post:
      summary: Report (App Id authentication pattern)
      description: Report (app id authentication pattern).
      operationId: report
      x-api-path-slug: transactions-xml-post
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: service_id
        description: Service id
      - in: query
        name: transactions
        description: Transactions to be reported
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Xml
  /transactions/authorize.xml:
    get:
      summary: Authorize (App Id authentication pattern)
      description: Authorize (app id authentication pattern).
      operationId: authorize
      x-api-path-slug: transactionsauthorize-xml-get
      parameters:
      - in: query
        name: app_id
        description: App Id (identifier of the application if the auth
      - in: query
        name: app_key
        description: App Key (shared secret of the application if the authentication
          pattern is App Id)
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: referrer
        description: Referrer IP Address or Domain
      - in: query
        name: service_id
        description: Service id
      - in: query
        name: usage
        description: Predicted Usage
      - in: query
        name: user_id
        description: User id
      - in: query
        name: user_key
        description: User Key (identifier and shared secret of the application if
          the auth
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Authorize
      - Xml
  /transactions/authrep.xml:
    get:
      summary: AuthRep (Authorize + Report for the App Id authentication pattern)
      description: Authrep (authorize + report for the app id authentication pattern).
      operationId: authrep
      x-api-path-slug: transactionsauthrep-xml-get
      parameters:
      - in: query
        name: app_id
        description: App Id (identifier of the application if the auth
      - in: query
        name: app_key
        description: App Key (shared secret of the application if the authentication
          pattern is App Id)
      - in: query
        name: log
        description: Request Log allows to log the requests/responses/status_codes
          of your API back to 3scale to maintain a log of the latest activity on your
          API
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: referrer
        description: Referrer IP Address or Domain
      - in: query
        name: service_id
        description: Service id
      - in: query
        name: usage
        description: Usage will increment the metrics with the values passed
      - in: query
        name: user_id
        description: User id
      - in: query
        name: user_key
        description: User Key (identifier and shared secret of the application if
          the auth
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Authrep
      - Xml
  /transactions/oauth_authorize.xml:
    get:
      summary: Authorize (Oauth authentication mode pattern)
      description: Authorize (oauth authentication mode pattern).
      operationId: authorize
      x-api-path-slug: transactionsoauth-authorize-xml-get
      parameters:
      - in: query
        name: app_id
        description: Client Id (identifier of the application if the auth
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: redirect_url
        description: Optional redirect URL for OAuth
      - in: query
        name: referrer
        description: Referrer IP Address or Domain
      - in: query
        name: service_id
        description: Service id
      - in: query
        name: usage
        description: Predicted Usage
      - in: query
        name: user_id
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Oauth
      - Authorize
      - Xml
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