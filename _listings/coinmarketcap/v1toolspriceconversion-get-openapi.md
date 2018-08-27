---
swagger: "2.0"
x-collection-name: CoinMarketCap
x-complete: 0
info:
  title: CoinMarketCap Price conversion tool
  description: |-
    Convert an amount of one currency into up to 32 other cryptocurrency or fiat currencies at the same time using latest exchange rates. Optionally pass a historical timestamp to convert values based on historic averages.

    **Note:** Historical fiat conversions aren't yet available and the latest fiat rates will be used as noted by the `last_updated` timestamp included in the market quote. Historical fiat rates will be coming soon.

    **This endpoint is available on the following API plans:**
    - ~~Starter~~
    - Hobbyist
    - Standard
    - Professional
    - Enterprise

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  termsOfService: https://coinmarketcap.com/terms/
  version: 1.0.0
host: pro-api.coinmarketcap.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/tools/price-conversion:
    get:
      summary: Price conversion tool
      description: |-
        Convert an amount of one currency into up to 32 other cryptocurrency or fiat currencies at the same time using latest exchange rates. Optionally pass a historical timestamp to convert values based on historic averages.

        **Note:** Historical fiat conversions aren't yet available and the latest fiat rates will be used as noted by the `last_updated` timestamp included in the market quote. Historical fiat rates will be coming soon.

        **This endpoint is available on the following API plans:**
        - ~~Starter~~
        - Hobbyist
        - Standard
        - Professional
        - Enterprise

        **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
      operationId: getV1ToolsPriceconversion
      x-api-path-slug: v1toolspriceconversion-get
      parameters:
      - in: query
        name: amount
        description: An amount of currency to convert
      - in: query
        name: convert
        description: Pass up to 32 comma-separated fiat or cryptocurrency symbols
          to convert the source amount to
      - in: query
        name: id
        description: The CoinMarketCap cryptocurrency ID of the base currency to convert
          from
      - in: query
        name: symbol
        description: Alternatively the cryptocurrency symbol of the base currency
          to convert from
      - in: query
        name: time
        description: Optional timestamp (Unix or ISO 8601) to reference historical
          pricing during conversion
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Price
      - Conversion
      - Tool
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