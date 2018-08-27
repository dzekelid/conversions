swagger: "2.0"
x-collection-name: Blockchain
x-complete: 1
info:
  title: Blockchain
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tobtc:
    get:
      summary: Convert
      description: Convert x value in the provided currency to btc.
      operationId: convertToBTC
      x-api-path-slug: tobtc-get
      parameters:
      - in: query
        name: currency
        description: A currency code
        type: string
        format: string
      - in: query
        name: value
        description: Value to convert
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Conversion