---
name: 3scale
x-slug: 3scale
description: 3scales API Management platform gives you the tools you need to take
  control of your API. Trusted by more customers than any other vendor.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
x-kinRank: "10"
x-alexaRank: "345437"
tags: 3scale
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apis.md
specificationVersion: "0.14"
apis:
- name: 3Scale Account Management API Account List
  x-api-slug: 3scale-account-management-api
  description: Account list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts.xml
  tags: Account,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccounts-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccounts-xml-get-openapi.md
- name: 3Scale Account Management API Account Find
  x-api-slug: 3scale-account-management-api
  description: Account find.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/find.xml
  tags: Account,Find
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsfind-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsfind-xml-get-openapi.md
- name: 3Scale Account Management API Application List
  x-api-slug: 3scale-account-management-api
  description: Application list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications.xml
  tags: Application,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-get-openapi.md
- name: 3Scale Account Management API Application Create
  x-api-slug: 3scale-account-management-api
  description: Application create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications.xml
  tags: Application,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplications-xml-post-openapi.md
- name: 3Scale Account Management API Application Key List
  x-api-slug: 3scale-account-management-api
  description: Application key list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{application_id}/keys.xml
  tags: Application,Key,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-get-openapi.md
- name: 3Scale Account Management API Application key Create
  x-api-slug: 3scale-account-management-api
  description: Application key create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{application_id}/keys.xml
  tags: Application,Key,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-post-openapi.md
- name: 3Scale Account Management API Application key Delete
  x-api-slug: 3scale-account-management-api
  description: Application key delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{application_id}/keys/{key}.xml
  tags: Application,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeyskey-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idkeyskey-xml-delete-openapi.md
- name: 3Scale Account Management API Application Referrer Filter List
  x-api-slug: 3scale-account-management-api
  description: Application referrer filter list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{application_id}/referrer_filters.xml
  tags: Application,Referrer,Filter,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-get-openapi.md
- name: 3Scale Account Management API Application referrer filter Create
  x-api-slug: 3scale-account-management-api
  description: Application referrer filter create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{application_id}/referrer_filters.xml
  tags: Application,Referrer,Filter,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-post-openapi.md
- name: 3Scale Account Management API Application referrer filter Delete
  x-api-slug: 3scale-account-management-api
  description: Application referrer filter delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{application_id}/referrer_filters/{id}.xml
  tags: Application,Referrer,Filter
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filtersid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsapplication-idreferrer-filtersid-xml-delete-openapi.md
- name: 3Scale Account Management API Application Read
  x-api-slug: 3scale-account-management-api
  description: Application read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}.xml
  tags: Application,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-get-openapi.md
- name: 3Scale Account Management API Application Update
  x-api-slug: 3scale-account-management-api
  description: Application update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}.xml
  tags: Application
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsid-xml-put-openapi.md
- name: 3Scale Account Management API Application Accept
  x-api-slug: 3scale-account-management-api
  description: Application accept.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}/accept.xml
  tags: Application,Accept
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidaccept-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidaccept-xml-put-openapi.md
- name: 3Scale Account Management API Application Change Plan
  x-api-slug: 3scale-account-management-api
  description: Application change plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}/change_plan.xml
  tags: Application,Change,Plan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidchange-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidchange-plan-xml-put-openapi.md
- name: 3Scale Account Management API Application Create Plan Customization
  x-api-slug: 3scale-account-management-api
  description: Application create plan customization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}/customize_plan.xml
  tags: Application,Plan,Customization
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidcustomize-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidcustomize-plan-xml-put-openapi.md
- name: 3Scale Account Management API Application Delete Plan Customization
  x-api-slug: 3scale-account-management-api
  description: Application delete plan customization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}/decustomize_plan.xml
  tags: Application,,Plan,Customization
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsiddecustomize-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsiddecustomize-plan-xml-put-openapi.md
- name: 3Scale Account Management API Application Resume
  x-api-slug: 3scale-account-management-api
  description: Application resume.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}/resume.xml
  tags: Application,Resume
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidresume-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidresume-xml-put-openapi.md
- name: 3Scale Account Management API Application Suspend
  x-api-slug: 3scale-account-management-api
  description: Application suspend.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/applications/{id}/suspend.xml
  tags: Application,Suspend
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidsuspend-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idapplicationsidsuspend-xml-put-openapi.md
- name: 3Scale Account Management API Account Message
  x-api-slug: 3scale-account-management-api
  description: Account message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/messages.xml
  tags: Account,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idmessages-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idmessages-xml-post-openapi.md
- name: 3Scale Account Management API Account Fetch Account Plan
  x-api-slug: 3scale-account-management-api
  description: Account fetch account plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/plan.xml
  tags: Account,Fetch,Account,Plan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idplan-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idplan-xml-get-openapi.md
- name: 3Scale Account Management API User List
  x-api-slug: 3scale-account-management-api
  description: User list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users.xml
  tags: User,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-get-openapi.md
- name: 3Scale Account Management API User Create
  x-api-slug: 3scale-account-management-api
  description: User create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users.xml
  tags: User,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusers-xml-post-openapi.md
- name: 3Scale Account Management API User Delete
  x-api-slug: 3scale-account-management-api
  description: User delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}.xml
  tags: User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-delete-openapi.md
- name: 3Scale Account Management API User Read
  x-api-slug: 3scale-account-management-api
  description: User read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}.xml
  tags: User,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-get-openapi.md
- name: 3Scale Account Management API User Update
  x-api-slug: 3scale-account-management-api
  description: User update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}.xml
  tags: User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersid-xml-put-openapi.md
- name: 3Scale Account Management API User Activate
  x-api-slug: 3scale-account-management-api
  description: User activate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}/activate.xml
  tags: User,Activate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidactivate-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidactivate-xml-put-openapi.md
- name: 3Scale Account Management API User change Role to Admin
  x-api-slug: 3scale-account-management-api
  description: User change role to admin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}/admin.xml
  tags: User,Change,Role,To,Admin
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidadmin-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidadmin-xml-put-openapi.md
- name: 3Scale Account Management API User change Role to Member
  x-api-slug: 3scale-account-management-api
  description: User change role to member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}/member.xml
  tags: User,Change,Role,To,Member
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidmember-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidmember-xml-put-openapi.md
- name: 3Scale Account Management API User Suspend
  x-api-slug: 3scale-account-management-api
  description: User suspend.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}/suspend.xml
  tags: User,Suspend
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidsuspend-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidsuspend-xml-put-openapi.md
- name: 3Scale Account Management API User Unsuspend
  x-api-slug: 3scale-account-management-api
  description: User unsuspend.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{account_id}/users/{id}/unsuspend.xml
  tags: User,Unsuspend
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidunsuspend-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsaccount-idusersidunsuspend-xml-put-openapi.md
- name: 3Scale Account Management API Account Delete
  x-api-slug: 3scale-account-management-api
  description: Account delete .
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}.xml
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-delete-openapi.md
- name: 3Scale Account Management API Account Read
  x-api-slug: 3scale-account-management-api
  description: Account read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}.xml
  tags: Account,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-get-openapi.md
- name: 3Scale Account Management API Account Update
  x-api-slug: 3scale-account-management-api
  description: Account update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}.xml
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsid-xml-put-openapi.md
- name: 3Scale Account Management API Account Approve
  x-api-slug: 3scale-account-management-api
  description: Account approve.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}/approve.xml
  tags: Account,Approve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidapprove-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidapprove-xml-put-openapi.md
- name: 3Scale Account Management API Account Change Plan
  x-api-slug: 3scale-account-management-api
  description: Account change plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}/change_plan.xml
  tags: Account,Change,Plan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidchange-plan-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidchange-plan-xml-put-openapi.md
- name: 3Scale Account Management API Account Delete Credit Card
  x-api-slug: 3scale-account-management-api
  description: Account delete credit card.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}/credit_card.xml
  tags: Account,,Credit,Card
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-delete-openapi.md
- name: 3Scale Account Management API Account Set Credit Card
  x-api-slug: 3scale-account-management-api
  description: Account set credit card.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}/credit_card.xml
  tags: Account,Set,Credit,Card
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidcredit-card-xml-put-openapi.md
- name: 3Scale Account Management API Account Reset to Pending
  x-api-slug: 3scale-account-management-api
  description: Account reset to pending.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}/make_pending.xml
  tags: Account,Reset,To,Pending
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidmake-pending-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidmake-pending-xml-put-openapi.md
- name: 3Scale Account Management API Account Reject
  x-api-slug: 3scale-account-management-api
  description: Account reject.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/accounts/{id}/reject.xml
  tags: Account,Reject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidreject-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccountsidreject-xml-put-openapi.md
- name: 3Scale Account Management API Account Plan List
  x-api-slug: 3scale-account-management-api
  description: Account plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans.xml
  tags: Account,Plan,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-get-openapi.md
- name: 3Scale Account Management API Account Plan Create
  x-api-slug: 3scale-account-management-api
  description: Account plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans.xml
  tags: Account,Plan,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plans-xml-post-openapi.md
- name: 3Scale Account Management API Account Plan Feature List
  x-api-slug: 3scale-account-management-api
  description: Account plan feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{account_plan_id}/features.xml
  tags: Account,Plan,Feature,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeatures-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API Account Plan Features Delete
  x-api-slug: 3scale-account-management-api
  description: Account plan features delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{account_plan_id}/features/{id}.xml
  tags: Account,Plan,Features
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API Account Plan Features Create
  x-api-slug: 3scale-account-management-api
  description: Account plan features create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{account_plan_id}/features/{id}.xml
  tags: Account,Plan,Features,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansaccount-plan-idfeaturesid-xml-post-openapi.md
- name: 3Scale Account Management API Account Plan Delete
  x-api-slug: 3scale-account-management-api
  description: Account plan delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{id}.xml
  tags: Account,Plan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-delete-openapi.md
- name: 3Scale Account Management API Account Plan Read
  x-api-slug: 3scale-account-management-api
  description: Account plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{id}.xml
  tags: Account,Plan,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-get-openapi.md
- name: 3Scale Account Management API Account Plan Update
  x-api-slug: 3scale-account-management-api
  description: Account plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{id}.xml
  tags: Account,Plan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansid-xml-put-openapi.md
- name: 3Scale Account Management API Account Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: Account plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{id}/default.xml
  tags: Account,Plan,Set,To,Default
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansiddefault-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiaccount-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API ActiveDocs JSON Spec Update
  x-api-slug: 3scale-account-management-api
  description: Activedocs json spec update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/active_docs/{id}.xml
  tags: ActiveDocs,JSON,Spec
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiactive-docsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiactive-docsid-xml-put-openapi.md
- name: 3Scale Account Management API Application List (all services)
  x-api-slug: 3scale-account-management-api
  description: Application list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/applications.xml
  tags: Application,List,(all,Services)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplications-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplications-xml-get-openapi.md
- name: 3Scale Account Management API Application Find
  x-api-slug: 3scale-account-management-api
  description: Application find.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/applications/find.xml
  tags: Application,Find
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplicationsfind-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplicationsfind-xml-get-openapi.md
- name: 3Scale Account Management API Application Plan List (all services)
  x-api-slug: 3scale-account-management-api
  description: Application plan list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans.xml
  tags: Application,Plan,List,(all,Services)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plans-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plans-xml-get-openapi.md
- name: 3Scale Account Management API Application Plan Feature List
  x-api-slug: 3scale-account-management-api
  description: Application plan feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/features.xml
  tags: Application,Plan,Feature,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API Application Plan Feature Create
  x-api-slug: 3scale-account-management-api
  description: Application plan feature create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/features.xml
  tags: Application,Plan,Feature,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeatures-xml-post-openapi.md
- name: 3Scale Account Management API Application Plan Feature Delete
  x-api-slug: 3scale-account-management-api
  description: Application plan feature delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/features/{id}.xml
  tags: Application,Plan,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API Limits List per Application Plan
  x-api-slug: 3scale-account-management-api
  description: Limits list per application plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/limits.xml
  tags: Limits,List,Per,Application,Plan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idlimits-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idlimits-xml-get-openapi.md
- name: 3Scale Account Management API Limit List per Metric
  x-api-slug: 3scale-account-management-api
  description: Limit list per metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits.xml
  tags: Limit,List,Per,Metric
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-get-openapi.md
- name: 3Scale Account Management API Limit Create
  x-api-slug: 3scale-account-management-api
  description: Limit create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits.xml
  tags: Limit,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-post-openapi.md
- name: 3Scale Account Management API Limit Delete
  x-api-slug: 3scale-account-management-api
  description: Limit delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits/{id}.xml
  tags: Limit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-delete-openapi.md
- name: 3Scale Account Management API Limit Read
  x-api-slug: 3scale-account-management-api
  description: Limit read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits/{id}.xml
  tags: Limit,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-get-openapi.md
- name: 3Scale Account Management API Limit Update
  x-api-slug: 3scale-account-management-api
  description: Limit update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits/{id}.xml
  tags: Limit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idlimitsid-xml-put-openapi.md
- name: 3Scale Account Management API Pricing Rules List per Metric
  x-api-slug: 3scale-account-management-api
  description: Pricing rules list per metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/pricing_rules.xml
  tags: Pricing,Rules,List,Per,Metric
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idpricing-rules-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idmetricsmetric-idpricing-rules-xml-get-openapi.md
- name: 3Scale Account Management API Pricing Rules List per Application Plan
  x-api-slug: 3scale-account-management-api
  description: Pricing rules list per application plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/application_plans/{application_plan_id}/pricing_rules.xml
  tags: Pricing,Rules,List,Per,Application,Plan
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idpricing-rules-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiapplication-plansapplication-plan-idpricing-rules-xml-get-openapi.md
- name: 3Scale Account Management API End User Plan List (all services)
  x-api-slug: 3scale-account-management-api
  description: End user plan list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/end_user_plans.xml
  tags: End,User,Plan,List,(all,Services)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plans-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plans-xml-get-openapi.md
- name: 3Scale Account Management API Limit List for End User Plans
  x-api-slug: 3scale-account-management-api
  description: Limit list for end user plans .
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits.xml
  tags: Limit,ListEnd,User,Plans
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get-openapi.md
- name: 3Scale Account Management API Limit Create for End User Plans
  x-api-slug: 3scale-account-management-api
  description: Limit create for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits.xml
  tags: Limit,CreateEnd,User,Plans
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-post-openapi.md
- name: 3Scale Account Management API Limit Delete for End User Plans
  x-api-slug: 3scale-account-management-api
  description: Limit delete for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits/{id}.xml
  tags: Limit,End,User,Plans
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete-openapi.md
- name: 3Scale Account Management API Limit Read for End User Plans
  x-api-slug: 3scale-account-management-api
  description: Limit read for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits/{id}.xml
  tags: Limit,ReadEnd,User,Plans
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-get-openapi.md
- name: 3Scale Account Management API Limit Update for End User Plans
  x-api-slug: 3scale-account-management-api
  description: Limit update for end user plans.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits/{id}.xml
  tags: Limit,End,User,Plans
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put-openapi.md
- name: 3Scale Account Management API Account Feature List
  x-api-slug: 3scale-account-management-api
  description: Account feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/features.xml
  tags: Account,Feature,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-get-openapi.md
- name: 3Scale Account Management API Account Feature Create
  x-api-slug: 3scale-account-management-api
  description: Account feature create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/features.xml
  tags: Account,Feature,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeatures-xml-post-openapi.md
- name: 3Scale Account Management API Account Feature Delete
  x-api-slug: 3scale-account-management-api
  description: Account feature delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/features/{id}.xml
  tags: Account,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API Account Feature Read
  x-api-slug: 3scale-account-management-api
  description: Account feature read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/features/{id}.xml
  tags: Account,Feature,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-get-openapi.md
- name: 3Scale Account Management API Account Feature Update
  x-api-slug: 3scale-account-management-api
  description: Account feature update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/features/{id}.xml
  tags: Account,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapifeaturesid-xml-put-openapi.md
- name: 3Scale Account Management API Nginx configuration files
  x-api-slug: 3scale-account-management-api
  description: Nginx configuration files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/nginx.zip
  tags: Nginx,Configuration,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapinginx-zip-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapinginx-zip-get-openapi.md
- name: 3Scale Account Management API Account Read
  x-api-slug: 3scale-account-management-api
  description: Account read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/provider.xml
  tags: Account,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiprovider-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiprovider-xml-get-openapi.md
- name: 3Scale Account Management API Service List
  x-api-slug: 3scale-account-management-api
  description: Service list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services.xml
  tags: Service,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservices-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservices-xml-get-openapi.md
- name: 3Scale Account Management API Service Create
  x-api-slug: 3scale-account-management-api
  description: Service create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services.xml
  tags: Service,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservices-xml-post-openapi.md
- name: 3Scale Account Management API Service Read
  x-api-slug: 3scale-account-management-api
  description: Service read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{id}.xml
  tags: Service,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesid-xml-get-openapi.md
- name: 3Scale Account Management API Service Update
  x-api-slug: 3scale-account-management-api
  description: Service update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{id}.xml
  tags: Service
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesid-xml-put-openapi.md
- name: 3Scale Account Management API Service Plan List
  x-api-slug: 3scale-account-management-api
  description: Service plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{id}/service_plans.xml
  tags: Service,Plan,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesidservice-plans-xml-get-openapi.md
- name: 3Scale Account Management API Service Plan Create
  x-api-slug: 3scale-account-management-api
  description: Service plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{id}/service_plans.xml
  tags: Service,Plan,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesidservice-plans-xml-post-openapi.md
- name: 3Scale Account Management API Application Plan List
  x-api-slug: 3scale-account-management-api
  description: Application plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/application_plans.xml
  tags: Application,Plan,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plans-xml-get-openapi.md
- name: 3Scale Account Management API Application Plan Create
  x-api-slug: 3scale-account-management-api
  description: Application plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/application_plans.xml
  tags: Application,Plan,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plans-xml-post-openapi.md
- name: 3Scale Account Management API Application Plan Delete
  x-api-slug: 3scale-account-management-api
  description: Application plan delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/application_plans/{id}.xml
  tags: Application,Plan
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansid-xml-delete-openapi.md
- name: 3Scale Account Management API Application Plan Read
  x-api-slug: 3scale-account-management-api
  description: Application plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/application_plans/{id}.xml
  tags: Application,Plan,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansid-xml-get-openapi.md
- name: 3Scale Account Management API Application Plan Update
  x-api-slug: 3scale-account-management-api
  description: Application plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/application_plans/{id}.xml
  tags: Application,Plan
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansid-xml-put-openapi.md
- name: 3Scale Account Management API Application Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: Application plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/application_plans/{id}/default.xml
  tags: Application,Plan,Set,To,Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idapplication-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API End User Create
  x-api-slug: 3scale-account-management-api
  description: End user create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_users.xml
  tags: End,User,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-users-xml-post-openapi.md
- name: 3Scale Account Management API End User Delete
  x-api-slug: 3scale-account-management-api
  description: End user delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_users/{username}.xml
  tags: End,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-usersusername-xml-delete-openapi.md
- name: 3Scale Account Management API End User Read
  x-api-slug: 3scale-account-management-api
  description: End user read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_users/{username}.xml
  tags: End,User,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-usersusername-xml-get-openapi.md
- name: 3Scale Account Management API End User Change Plan
  x-api-slug: 3scale-account-management-api
  description: End user change plan.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_users/{username}/change_plan.xml
  tags: End,User,Change,Plan
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-usersusernamechange-plan-xml-put-openapi.md
- name: 3Scale Account Management API End User Plan List
  x-api-slug: 3scale-account-management-api
  description: End user plan list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_user_plans.xml
  tags: End,User,Plan,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plans-xml-get-openapi.md
- name: 3Scale Account Management API End User Plan Create
  x-api-slug: 3scale-account-management-api
  description: End user plan create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_user_plans.xml
  tags: End,User,Plan,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plans-xml-post-openapi.md
- name: 3Scale Account Management API End User Plan Read
  x-api-slug: 3scale-account-management-api
  description: End user plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_user_plans/{id}.xml
  tags: End,User,Plan,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plansid-xml-get-openapi.md
- name: 3Scale Account Management API End User Plan Update
  x-api-slug: 3scale-account-management-api
  description: End user plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_user_plans/{id}.xml
  tags: End,User,Plan
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plansid-xml-put-openapi.md
- name: 3Scale Account Management API End User Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: End user plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_user_plans/{id}/default.xml
  tags: End,User,Plan,Set,To,Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idend-user-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API Service Feature List
  x-api-slug: 3scale-account-management-api
  description: Service feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/features.xml
  tags: Service,Feature,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API Service Feature Create
  x-api-slug: 3scale-account-management-api
  description: Service feature create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/features.xml
  tags: Service,Feature,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeatures-xml-post-openapi.md
- name: 3Scale Account Management API Service Feature Delete
  x-api-slug: 3scale-account-management-api
  description: Service feature delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/features/{id}.xml
  tags: Service,Feature
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeaturesid-xml-delete-openapi.md
- name: 3Scale Account Management API Service Feature Read
  x-api-slug: 3scale-account-management-api
  description: Service feature read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/features/{id}.xml
  tags: Service,Feature,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeaturesid-xml-get-openapi.md
- name: 3Scale Account Management API Service Feature Update
  x-api-slug: 3scale-account-management-api
  description: Service feature update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/features/{id}.xml
  tags: Service,Feature
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idfeaturesid-xml-put-openapi.md
- name: 3Scale Account Management API Metric List
  x-api-slug: 3scale-account-management-api
  description: Metric list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics.xml
  tags: Metric,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetrics-xml-get-openapi.md
- name: 3Scale Account Management API Metric Create
  x-api-slug: 3scale-account-management-api
  description: Metric create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics.xml
  tags: Metric,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetrics-xml-post-openapi.md
- name: 3Scale Account Management API Metric Delete
  x-api-slug: 3scale-account-management-api
  description: Metric delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{id}.xml
  tags: Metric
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsid-xml-delete-openapi.md
- name: 3Scale Account Management API Metric Read
  x-api-slug: 3scale-account-management-api
  description: Metric read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{id}.xml
  tags: Metric,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsid-xml-get-openapi.md
- name: 3Scale Account Management API Metric Update
  x-api-slug: 3scale-account-management-api
  description: Metric update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{id}.xml
  tags: Metric
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsid-xml-put-openapi.md
- name: 3Scale Account Management API Method List
  x-api-slug: 3scale-account-management-api
  description: Method list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{metric_id}/methods.xml
  tags: Method,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethods-xml-get-openapi.md
- name: 3Scale Account Management API Method Create
  x-api-slug: 3scale-account-management-api
  description: Method create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{metric_id}/methods.xml
  tags: Method,Create
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethods-xml-post-openapi.md
- name: 3Scale Account Management API Method Delete
  x-api-slug: 3scale-account-management-api
  description: Method delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{metric_id}/methods/{id}.xml
  tags: Method
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethodsid-xml-delete-openapi.md
- name: 3Scale Account Management API Method Read
  x-api-slug: 3scale-account-management-api
  description: Method read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{metric_id}/methods/{id}.xml
  tags: Method,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethodsid-xml-get-openapi.md
- name: 3Scale Account Management API Method Update
  x-api-slug: 3scale-account-management-api
  description: Method update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/metrics/{metric_id}/methods/{id}.xml
  tags: Method
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idmetricsmetric-idmethodsid-xml-put-openapi.md
- name: 3Scale Account Management API Service Plan Delete
  x-api-slug: 3scale-account-management-api
  description: Service plan delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/service_plans/{id}.xml
  tags: Service,Plan
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansid-xml-delete-openapi.md
- name: 3Scale Account Management API Service Plan Read
  x-api-slug: 3scale-account-management-api
  description: Service plan read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/service_plans/{id}.xml
  tags: Service,Plan,Read
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansid-xml-get-openapi.md
- name: 3Scale Account Management API Service Plan Update
  x-api-slug: 3scale-account-management-api
  description: Service plan update.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/service_plans/{id}.xml
  tags: Service,Plan
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansid-xml-put-openapi.md
- name: 3Scale Account Management API Service Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: Service plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/service_plans/{id}/default.xml
  tags: Service,Plan,Set,To,Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservicesservice-idservice-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API Service Plan List (all services)
  x-api-slug: 3scale-account-management-api
  description: Service plan list (all services).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/service_plans.xml
  tags: Service,Plan,List,(all,Services)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservice-plans-xml-get-openapi.md
- name: 3Scale Account Management API Service Plan Feature List
  x-api-slug: 3scale-account-management-api
  description: Service plan feature list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/service_plans/{service_plan_id}/features.xml
  tags: Service,Plan,Feature,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservice-plansservice-plan-idfeatures-xml-get-openapi.md
- name: 3Scale Account Management API Service Plan Feature Add
  x-api-slug: 3scale-account-management-api
  description: Service plan feature add.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/service_plans/{service_plan_id}/features.xml
  tags: Service,Plan,Feature
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiservice-plansservice-plan-idfeatures-xml-post-openapi.md
- name: 3Scale Account Management API Signup Express
  x-api-slug: 3scale-account-management-api
  description: Signup express.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/signup.xml
  tags: Signup,Express
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapisignup-xml-post-openapi.md
- name: 3Scale Account Management API User List (provider account)
  x-api-slug: 3scale-account-management-api
  description: User list (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users.xml
  tags: User,List,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusers-xml-get-openapi.md
- name: 3Scale Account Management API User Create (provider account)
  x-api-slug: 3scale-account-management-api
  description: User create (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users.xml
  tags: User,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusers-xml-post-openapi.md
- name: 3Scale Account Management API User Delete (provider account)
  x-api-slug: 3scale-account-management-api
  description: User delete (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}.xml
  tags: User,,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersid-xml-delete-openapi.md
- name: 3Scale Account Management API User Read (provider account)
  x-api-slug: 3scale-account-management-api
  description: User read (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}.xml
  tags: User,Read,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersid-xml-get-openapi.md
- name: 3Scale Account Management API User Update (provider account)
  x-api-slug: 3scale-account-management-api
  description: User update (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}.xml
  tags: User,,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersid-xml-put-openapi.md
- name: 3Scale Account Management API User Activate (provider account)
  x-api-slug: 3scale-account-management-api
  description: User activate (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}/activate.xml
  tags: User,Activate,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidactivate-xml-put-openapi.md
- name: 3Scale Account Management API User change Role to Admin (provider account)
  x-api-slug: 3scale-account-management-api
  description: User change role to admin (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}/admin.xml
  tags: User,Change,Role,To,Admin,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidadmin-xml-put-openapi.md
- name: 3Scale Account Management API User change Role to Member (provider account)
  x-api-slug: 3scale-account-management-api
  description: User change role to member (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}/member.xml
  tags: User,Change,Role,To,Member,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidmember-xml-put-openapi.md
- name: 3Scale Account Management API User Suspend (provider account)
  x-api-slug: 3scale-account-management-api
  description: User suspend (provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}/suspend.xml
  tags: User,Suspend,(provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidsuspend-xml-put-openapi.md
- name: 3Scale Account Management API User Unsuspend (of provider account)
  x-api-slug: 3scale-account-management-api
  description: User unsuspend (of provider account).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/users/{id}/unsuspend.xml
  tags: User,Unsuspend,(of,Provider,Account)
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiusersidunsuspend-xml-put-openapi.md
- name: 3Scale Account Management API Webhooks Delete Failed Deliveries
  x-api-slug: 3scale-account-management-api
  description: Webhooks delete failed deliveries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/webhooks/failures.xml
  tags: Webhooks,,Failed,Deliveries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiwebhooksfailures-xml-delete-openapi.md
- name: 3Scale Account Management API Webhooks List Failed Deliveries
  x-api-slug: 3scale-account-management-api
  description: Webhooks list failed deliveries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/webhooks/failures.xml
  tags: Webhooks,List,Failed,Deliveries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/adminapiwebhooksfailures-xml-get-openapi.md
- name: 3Scale Account Management API
  x-api-slug: 3scale-account-management-api
  description: 3scales API Management platform gives you the tools you need to take
    control of your API. Trusted by more customers than any other vendor.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: 3scale
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/openapi.md
- name: 3Scale Analytics API Application Usage by Metric
  x-api-slug: 3scale-analytics-api
  description: Application usage by metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////stats/applications/{application_id}/usage.{format}
  tags: Application,Usage,By,Metric
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsapplicationsapplication-idusage-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsapplicationsapplication-idusage-format-get-openapi.md
- name: 3Scale Analytics API Service Top Applications
  x-api-slug: 3scale-analytics-api
  description: Service top applications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////stats/services/{service_id}/top_applications.{format}
  tags: Service,Top,Applications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idtop-applications-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idtop-applications-format-get-openapi.md
- name: 3Scale Analytics API Service Usage by Metric
  x-api-slug: 3scale-analytics-api
  description: Service usage by metric.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////stats/services/{service_id}/usage.{format}
  tags: Service,Usage,By,Metric
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idusage-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/statsservicesservice-idusage-format-get-openapi.md
- name: 3Scale Analytics API
  x-api-slug: 3scale-analytics-api
  description: 3scales API Management platform gives you the tools you need to take
    control of your API. Trusted by more customers than any other vendor.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: 3scale
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/openapi.md
- name: 3Scale Billing API Invoice List by Account
  x-api-slug: 3scale-billing-api
  description: Invoice list by account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////api/accounts/{account_id}/invoices.xml
  tags: Invoice,List,By,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoices-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoices-xml-get-openapi.md
- name: 3Scale Billing API Invoice by Account
  x-api-slug: 3scale-billing-api
  description: Invoice by account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////api/accounts/{account_id}/invoices/{id}.xml
  tags: Invoice,By,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoicesid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiaccountsaccount-idinvoicesid-xml-get-openapi.md
- name: 3Scale Billing API Invoice List
  x-api-slug: 3scale-billing-api
  description: Invoice list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////api/invoices.xml
  tags: Invoice,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoices-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoices-xml-get-openapi.md
- name: 3Scale Billing API Invoice
  x-api-slug: 3scale-billing-api
  description: Invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////api/invoices/{id}.xml
  tags: Invoice
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesid-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesid-xml-get-openapi.md
- name: 3Scale Billing API Invoice
  x-api-slug: 3scale-billing-api
  description: Invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////api/invoices/{id}/state.xml
  tags: Invoice
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesidstate-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesidstate-xml-put-openapi.md
- name: 3Scale Billing API Invoice Line Items List
  x-api-slug: 3scale-billing-api
  description: Invoice line items list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////api/invoices/{invoice_id}/line_items.xml
  tags: Invoice,Line,Items,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idline-items-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idline-items-xml-get-openapi.md
- name: 3Scale Billing API Invoice Payment Transactions List
  x-api-slug: 3scale-billing-api
  description: Invoice payment transactions list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////api/invoices/{invoice_id}/payment_transactions.xml
  tags: Invoice,Payment,Transactions,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idpayment-transactions-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/apiinvoicesinvoice-idpayment-transactions-xml-get-openapi.md
- name: 3Scale Billing API
  x-api-slug: 3scale-billing-api
  description: 3scales API Management platform gives you the tools you need to take
    control of your API. Trusted by more customers than any other vendor.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: 3scale
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/openapi.md
- name: 3scale Service Management API Report (App Id authentication pattern)
  x-api-slug: 3scale-service-management-api
  description: Report (app id authentication pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////transactions.xml
  tags: Transactions,Xml
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactions-xml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactions-xml-post-openapi.md
- name: 3scale Service Management API Authorize (App Id authentication pattern)
  x-api-slug: 3scale-service-management-api
  description: Authorize (app id authentication pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////transactions/authorize.xml
  tags: Transactions,Authorize,Xml
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthorize-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthorize-xml-get-openapi.md
- name: 3scale Service Management API AuthRep (Authorize + Report for the App Id authentication
    pattern)
  x-api-slug: 3scale-service-management-api
  description: Authrep (authorize + report for the app id authentication pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////transactions/authrep.xml
  tags: Transactions,Authrep,Xml
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthrep-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsauthrep-xml-get-openapi.md
- name: 3scale Service Management API Authorize (Oauth authentication mode pattern)
  x-api-slug: 3scale-service-management-api
  description: Authorize (oauth authentication mode pattern).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////transactions/oauth_authorize.xml
  tags: Transactions,Oauth,Authorize,Xml
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsoauth-authorize-xml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/transactionsoauth-authorize-xml-get-openapi.md
- name: 3scale Service Management API
  x-api-slug: 3scale-service-management-api
  description: 3scales API Management platform gives you the tools you need to take
    control of your API. Trusted by more customers than any other vendor.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: 3scale
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/3scale/master/_listings/3scale/openapi.md
x-common:
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
  url: http://www.3scale.net
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---