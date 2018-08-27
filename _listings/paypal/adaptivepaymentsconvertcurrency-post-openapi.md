---
swagger: "2.0"
x-collection-name: PayPal
x-complete: 0
info:
  title: Paypal Convert Currency
  description: Use the ConvertCurrency API operation to request the current foreign
    exchange (FX) rate for a specific amount and currency.
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptivePayments/ConvertCurrency:
    post:
      summary: Convert Currency
      description: Use the ConvertCurrency API operation to request the current foreign
        exchange (FX) rate for a specific amount and currency.
      operationId: AdaptivePayments.ConvertCurrency.post
      x-api-path-slug: adaptivepaymentsconvertcurrency-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Currency
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