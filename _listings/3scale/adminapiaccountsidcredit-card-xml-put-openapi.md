---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Account Set Credit Card
  description: Account set credit card.
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
  /admin/api/accounts/{id}/credit_card.xml:
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