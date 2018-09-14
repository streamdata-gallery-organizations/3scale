---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Billing API Invoice List
  description: Invoice list.
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
  /api/invoices.xml:
    get:
      summary: Invoice List
      description: Invoice list.
      operationId: finance
      x-api-path-slug: apiinvoices-xml-get
      parameters:
      - in: query
        name: month
        description: Filter the invoice by month
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale
      - in: query
        name: state
        description: Filter the invoice by state
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - List
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