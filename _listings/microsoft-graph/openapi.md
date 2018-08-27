swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /workbook/tables(&lt;id|name&gt;)/convertToRange:
    post:
      summary: Table Convert To Range
      description: 'Table: convertToRange Converts the table into a normal range of
        cells. All data is preserved.'
      operationId: Table:ConvertToRange
      x-api-path-slug: workbooktablesltidnamegtconverttorange-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - ConvertRange
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/convertToRange:
    post:
      summary: Table Convert To Range
      description: 'Table: convertToRange Converts the table into a normal range of
        cells. All data is preserved.'
      operationId: Table:ConvertToRange
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtconverttorange-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - ConvertRange