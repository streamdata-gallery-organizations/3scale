---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API User Activate
  description: User activate.
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
  /admin/api/accounts.xml:
    get:
      summary: Account List
      description: Account list.
      operationId: account
      x-api-path-slug: adminapiaccounts-xml-get
      parameters:
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: state
        description: Account state
      responses:
        200:
          description: OK
      tags:
      - Account
      - List
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
  /admin/api/accounts/{account_id}/applications.xml:
    get:
      summary: Application List
      description: Application list.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplications-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - List
    post:
      summary: Application Create
      description: Application create.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplications-xml-post
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: query
        name: description
        description: Description of the application to be created
      - in: query
        name: name
        description: Name of the application to be created
      - in: query
        name: plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Create
  /admin/api/accounts/{account_id}/applications/{application_id}/keys.xml:
    get:
      summary: Application Key List
      description: Application key list.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Key
      - List
    post:
      summary: Application key Create
      description: Application key create.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-post
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: query
        name: key
        description: app_key to be added
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Key
      - Create
  /admin/api/accounts/{account_id}/applications/{application_id}/keys/{key}.xml:
    delete:
      summary: Application key Delete
      description: Application key delete.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idkeyskey-xml-delete
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: path
        name: key
        description: app_key to be deleted
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Key
  /admin/api/accounts/{account_id}/applications/{application_id}/referrer_filters.xml:
    get:
      summary: Application Referrer Filter List
      description: Application referrer filter list.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Referrer
      - Filter
      - List
    post:
      summary: Application referrer filter Create
      description: Application referrer filter create.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-post
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: referrer_filter
        description: referrer filter to be created
      responses:
        200:
          description: OK
      tags:
      - Application
      - Referrer
      - Filter
      - Create
  /admin/api/accounts/{account_id}/applications/{application_id}/referrer_filters/{id}.xml:
    delete:
      summary: Application referrer filter Delete
      description: Application referrer filter delete.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idreferrer-filtersid-xml-delete
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: path
        name: id
        description: id of referrer filter to be deleted
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Referrer
      - Filter
  /admin/api/accounts/{account_id}/applications/{id}.xml:
    get:
      summary: Application Read
      description: Application read.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsid-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Read
    put:
      summary: Application Update
      description: Application update.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsid-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: query
        name: description
        description: Description of the application
      - in: path
        name: id
        description: id of the application
      - in: query
        name: name
        description: Name of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
  /admin/api/accounts/{account_id}/applications/{id}/accept.xml:
    put:
      summary: Application Accept
      description: Application accept.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidaccept-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Accept
  /admin/api/accounts/{account_id}/applications/{id}/change_plan.xml:
    put:
      summary: Application Change Plan
      description: Application change plan.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidchange-plan-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: plan_id
        description: id of the new application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Change
      - Plan
  /admin/api/accounts/{account_id}/applications/{id}/customize_plan.xml:
    put:
      summary: Application Create Plan Customization
      description: Application create plan customization.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidcustomize-plan-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Customization
  /admin/api/accounts/{account_id}/applications/{id}/decustomize_plan.xml:
    put:
      summary: Application Delete Plan Customization
      description: Application delete plan customization.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsiddecustomize-plan-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - ""
      - Plan
      - Customization
  /admin/api/accounts/{account_id}/applications/{id}/resume.xml:
    put:
      summary: Application Resume
      description: Application resume.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidresume-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Resume
  /admin/api/accounts/{account_id}/applications/{id}/suspend.xml:
    put:
      summary: Application Suspend
      description: Application suspend.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidsuspend-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Suspend
  /admin/api/accounts/{account_id}/messages.xml:
    post:
      summary: Account Message
      description: Account message.
      operationId: account
      x-api-path-slug: adminapiaccountsaccount-idmessages-xml-post
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: body
        description: Text to send
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Message
  /admin/api/accounts/{account_id}/plan.xml:
    get:
      summary: Account Fetch Account Plan
      description: Account fetch account plan.
      operationId: account
      x-api-path-slug: adminapiaccountsaccount-idplan-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Fetch
      - Account
      - Plan
  /admin/api/accounts/{account_id}/users.xml:
    get:
      summary: User List
      description: User list.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusers-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: role
        description: Filter users by Role
      - in: query
        name: state
        description: Filter users by State
      responses:
        200:
          description: OK
      tags:
      - User
      - List
    post:
      summary: User Create
      description: User create.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusers-xml-post
      parameters:
      - in: path
        name: account_id
        description: id of the account
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
      - Create
  /admin/api/accounts/{account_id}/users/{id}.xml:
    delete:
      summary: User Delete
      description: User delete.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersid-xml-delete
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
    get:
      summary: User Read
      description: User read.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersid-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Read
    put:
      summary: User Update
      description: User update.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersid-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: query
        name: email
        description: Email of the user
      - in: path
        name: id
        description: id of the user
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
  /admin/api/accounts/{account_id}/users/{id}/activate.xml:
    put:
      summary: User Activate
      description: User activate.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersidactivate-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Activate
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