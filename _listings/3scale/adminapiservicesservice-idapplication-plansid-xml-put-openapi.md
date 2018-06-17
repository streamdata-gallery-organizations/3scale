---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Application Plan Update
  description: Application plan update.
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
  /admin/api/accounts/{account_id}/users/{id}/admin.xml:
    put:
      summary: User change Role to Admin
      description: User change role to admin.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersidadmin-xml-put
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
      - Change
      - Role
      - To
      - Admin
  /admin/api/accounts/{account_id}/users/{id}/member.xml:
    put:
      summary: User change Role to Member
      description: User change role to member.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersidmember-xml-put
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
      - Change
      - Role
      - To
      - Member
  /admin/api/accounts/{account_id}/users/{id}/suspend.xml:
    put:
      summary: User Suspend
      description: User suspend.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersidsuspend-xml-put
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
      - Suspend
  /admin/api/accounts/{account_id}/users/{id}/unsuspend.xml:
    put:
      summary: User Unsuspend
      description: User unsuspend.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersidunsuspend-xml-put
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
      - Unsuspend
  /admin/api/accounts/{id}.xml:
    delete:
      summary: Account Delete
      description: Account delete .
      operationId: account
      x-api-path-slug: adminapiaccountsid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Account Read
      description: Account read.
      operationId: account
      x-api-path-slug: adminapiaccountsid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Read
    put:
      summary: Account Update
      description: Account update.
      operationId: account
      x-api-path-slug: adminapiaccountsid-xml-put
      parameters:
      - in: query
        name: additional_fields
        description: Additional fields have to be name and value i
      - in: path
        name: id
        description: id of the account
      - in: query
        name: org_name
        description: Organization name of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
  /admin/api/accounts/{id}/approve.xml:
    put:
      summary: Account Approve
      description: Account approve.
      operationId: account
      x-api-path-slug: adminapiaccountsidapprove-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Approve
  /admin/api/accounts/{id}/change_plan.xml:
    put:
      summary: Account Change Plan
      description: Account change plan.
      operationId: account
      x-api-path-slug: adminapiaccountsidchange-plan-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: plan_id
        description: id of the target account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Change
      - Plan
  /admin/api/accounts/{id}/credit_card.xml:
    delete:
      summary: Account Delete Credit Card
      description: Account delete credit card.
      operationId: account
      x-api-path-slug: adminapiaccountsidcredit-card-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - ""
      - Credit
      - Card
    put:
      summary: Account Set Credit Card
      description: Account set credit card.
      operationId: account
      x-api-path-slug: adminapiaccountsidcredit-card-xml-put
      parameters:
      - in: query
        name: billing_address_address
        description: Address associated to the credit card
      - in: query
        name: billing_address_city
        description: Billing address city
      - in: query
        name: billing_address_country
        description: Billing address country
      - in: query
        name: billing_address_name
        description: Name of the person/company to bill
      - in: query
        name: billing_address_phone
        description: Billing address phone
      - in: query
        name: billing_address_state
        description: Billing address state
      - in: query
        name: billing_address_zip
        description: Billing address ZIP code
      - in: query
        name: credit_card_authorize_net_payment_profile_token
        description: Authorize
      - in: query
        name: credit_card_expiration_month
        description: Month of expiration of credit card
      - in: query
        name: credit_card_expiration_year
        description: Year of expiration of credit card
      - in: query
        name: credit_card_partial_number
        description: 4 last numbers of the credit card
      - in: query
        name: credit_card_token
        description: The token returned by the payment gateway
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Set
      - Credit
      - Card
  /admin/api/accounts/{id}/make_pending.xml:
    put:
      summary: Account Reset to Pending
      description: Account reset to pending.
      operationId: account
      x-api-path-slug: adminapiaccountsidmake-pending-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Reset
      - To
      - Pending
  /admin/api/accounts/{id}/reject.xml:
    put:
      summary: Account Reject
      description: Account reject.
      operationId: account
      x-api-path-slug: adminapiaccountsidreject-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Reject
  /admin/api/account_plans.xml:
    get:
      summary: Account Plan List
      description: Account plan list.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - List
    post:
      summary: Account Plan Create
      description: Account plan create.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plans-xml-post
      parameters:
      - in: query
        name: name
        description: Name of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Create
  /admin/api/account_plans/{account_plan_id}/features.xml:
    get:
      summary: Account Plan Feature List
      description: Account plan feature list.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeatures-xml-get
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Feature
      - List
  /admin/api/account_plans/{account_plan_id}/features/{id}.xml:
    delete:
      summary: Account Plan Features Delete
      description: Account plan features delete.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Features
    post:
      summary: Account Plan Features Create
      description: Account plan features create.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-post
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Features
      - Create
  /admin/api/account_plans/{id}.xml:
    delete:
      summary: Account Plan Delete
      description: Account plan delete.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
    get:
      summary: Account Plan Read
      description: Account plan read.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Read
    put:
      summary: Account Plan Update
      description: Account plan update.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: name
        description: Name of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
  /admin/api/account_plans/{id}/default.xml:
    put:
      summary: Account Plan set to Default
      description: Account plan set to default.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Set
      - To
      - Default
  /admin/api/active_docs/{id}.xml:
    put:
      summary: ActiveDocs JSON Spec Update
      description: Activedocs json spec update.
      operationId: active_docs
      x-api-path-slug: adminapiactive-docsid-xml-put
      parameters:
      - in: query
        name: body
        description: JSON Spec of the ActiveDocs (based on the spec of Swagger)
      - in: path
        name: id
        description: id of the active doc
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - ActiveDocs
      - JSON
      - Spec
  /admin/api/applications.xml:
    get:
      summary: Application List (all services)
      description: Application list (all services).
      operationId: application
      x-api-path-slug: adminapiapplications-xml-get
      parameters:
      - in: query
        name: active_since
        description: filter date
      - in: query
        name: inactive_since
        description: filter date
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
        name: service_id
        description: filter by service
      responses:
        200:
          description: OK
      tags:
      - Application
      - List
      - (all
      - Services)
  /admin/api/applications/find.xml:
    get:
      summary: Application Find
      description: Application find.
      operationId: application
      x-api-path-slug: adminapiapplicationsfind-xml-get
      parameters:
      - in: query
        name: application_id
        description: id of the application
      - in: query
        name: app_id
        description: app_id of the application (for app_id/app_key and oauth authentication
          modes)
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: user_key
        description: user_key of the application (for user_key authentication mode)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Find
  /admin/api/application_plans.xml:
    get:
      summary: Application Plan List (all services)
      description: Application plan list (all services).
      operationId: application_plan
      x-api-path-slug: adminapiapplication-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - List
      - (all
      - Services)
  /admin/api/application_plans/{application_plan_id}/features.xml:
    get:
      summary: Application Plan Feature List
      description: Application plan feature list.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeatures-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Feature
      - List
    post:
      summary: Application Plan Feature Create
      description: Application plan feature create.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeatures-xml-post
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: feature_id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Feature
      - Create
  /admin/api/application_plans/{application_plan_id}/features/{id}.xml:
    delete:
      summary: Application Plan Feature Delete
      description: Application plan feature delete.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Feature
  /admin/api/application_plans/{application_plan_id}/limits.xml:
    get:
      summary: Limits List per Application Plan
      description: Limits list per application plan.
      operationId: application_plan_limits
      x-api-path-slug: adminapiapplication-plansapplication-plan-idlimits-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limits
      - List
      - Per
      - Application
      - Plan
  /admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits.xml:
    get:
      summary: Limit List per Metric
      description: Limit list per metric.
      operationId: application_plan_limit
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - List
      - Per
      - Metric
    post:
      summary: Limit Create
      description: Limit create.
      operationId: application_plan_limit
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-post
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: period
        description: period of the limit
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: value
        description: value of the limit
      responses:
        200:
          description: OK
      tags:
      - Limit
      - Create
  /admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits/{id}.xml:
    delete:
      summary: Limit Delete
      description: Limit delete.
      operationId: application_plan_limit
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-delete
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
    get:
      summary: Limit Read
      description: Limit read.
      operationId: application_plan_limit
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - Read
    put:
      summary: Limit Update
      description: Limit update.
      operationId: application_plan_limit
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-put
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: period
        description: period of the limit
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: value
        description: value of the limit
      responses:
        200:
          description: OK
      tags:
      - Limit
  /admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/pricing_rules.xml:
    get:
      summary: Pricing Rules List per Metric
      description: Pricing rules list per metric.
      operationId: application_plan_pricing_rules
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idpricing-rules-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Pricing
      - Rules
      - List
      - Per
      - Metric
  /admin/api/application_plans/{application_plan_id}/pricing_rules.xml:
    get:
      summary: Pricing Rules List per Application Plan
      description: Pricing rules list per application plan.
      operationId: application_plan_pricing_rules
      x-api-path-slug: adminapiapplication-plansapplication-plan-idpricing-rules-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Pricing
      - Rules
      - List
      - Per
      - Application
      - Plan
  /admin/api/end_user_plans.xml:
    get:
      summary: End User Plan List (all services)
      description: End user plan list (all services).
      operationId: end_user_plan
      x-api-path-slug: adminapiend-user-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - List
      - (all
      - Services)
  /admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits.xml:
    get:
      summary: Limit List for End User Plans
      description: Limit list for end user plans .
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - ListEnd
      - User
      - Plans
    post:
      summary: Limit Create for End User Plans
      description: Limit create for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-post
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: period
        description: period of the limit
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: value
        description: value of the limit
      responses:
        200:
          description: OK
      tags:
      - Limit
      - CreateEnd
      - User
      - Plans
  /admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits/{id}.xml:
    delete:
      summary: Limit Delete for End User Plans
      description: Limit delete for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - End
      - User
      - Plans
    get:
      summary: Limit Read for End User Plans
      description: Limit read for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-get
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - ReadEnd
      - User
      - Plans
    put:
      summary: Limit Update for End User Plans
      description: Limit update for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: period
        description: period of the limit
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: value
        description: value of the limit
      responses:
        200:
          description: OK
      tags:
      - Limit
      - End
      - User
      - Plans
  /admin/api/features.xml:
    get:
      summary: Account Feature List
      description: Account feature list.
      operationId: account_feature
      x-api-path-slug: adminapifeatures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
      - List
    post:
      summary: Account Feature Create
      description: Account feature create.
      operationId: account_feature
      x-api-path-slug: adminapifeatures-xml-post
      parameters:
      - in: query
        name: name
        description: Name of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
      - Create
  /admin/api/features/{id}.xml:
    delete:
      summary: Account Feature Delete
      description: Account feature delete.
      operationId: account_feature
      x-api-path-slug: adminapifeaturesid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
    get:
      summary: Account Feature Read
      description: Account feature read.
      operationId: account_feature
      x-api-path-slug: adminapifeaturesid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
      - Read
    put:
      summary: Account Feature Update
      description: Account feature update.
      operationId: account_feature
      x-api-path-slug: adminapifeaturesid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: name
        description: Name of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
  /admin/api/nginx.zip:
    get:
      summary: Nginx configuration files
      description: Nginx configuration files.
      operationId: nginx
      x-api-path-slug: adminapinginx-zip-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Nginx
      - Configuration
      - Files
  /admin/api/provider.xml:
    get:
      summary: Account Read
      description: Account read.
      operationId: account
      x-api-path-slug: adminapiprovider-xml-get
      responses:
        200:
          description: OK
      tags:
      - Account
      - Read
  /admin/api/services.xml:
    get:
      summary: Service List
      description: Service list.
      operationId: service
      x-api-path-slug: adminapiservices-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - List
    post:
      summary: Service Create
      description: Service create.
      operationId: service
      x-api-path-slug: adminapiservices-xml-post
      parameters:
      - ~
      - in: query
        name: name
        description: Name of the service to be created
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Service
      - Create
  /admin/api/services/{id}.xml:
    get:
      summary: Service Read
      description: Service read.
      operationId: service
      x-api-path-slug: adminapiservicesid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the service
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - Read
    put:
      summary: Service Update
      description: Service update.
      operationId: service
      x-api-path-slug: adminapiservicesid-xml-put
      parameters:
      - ~
      - in: path
        name: id
        description: id of the service
      - in: query
        name: name
        description: New name for the service
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
  /admin/api/services/{id}/service_plans.xml:
    get:
      summary: Service Plan List
      description: Service plan list.
      operationId: service_plan
      x-api-path-slug: adminapiservicesidservice-plans-xml-get
      parameters:
      - in: path
        name: id
        description: id of the service
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - List
    post:
      summary: Service Plan Create
      description: Service plan create.
      operationId: service_plan
      x-api-path-slug: adminapiservicesidservice-plans-xml-post
      parameters:
      - in: path
        name: id
        description: id of the service
      - in: query
        name: name
        description: Name of the service plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Create
  /admin/api/services/{service_id}/application_plans.xml:
    get:
      summary: Application Plan List
      description: Application plan list.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - List
    post:
      summary: Application Plan Create
      description: Application plan create.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plans-xml-post
      parameters:
      - ~
      - in: query
        name: name
        description: Name of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Create
  /admin/api/services/{service_id}/application_plans/{id}.xml:
    delete:
      summary: Application Plan Delete
      description: Application plan delete.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
    get:
      summary: Application Plan Read
      description: Application plan read.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Read
    put:
      summary: Application Plan Update
      description: Application plan update.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansid-xml-put
      parameters:
      - ~
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: name
        description: Name of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
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