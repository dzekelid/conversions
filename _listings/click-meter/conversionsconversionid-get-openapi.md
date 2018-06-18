---
swagger: "2.0"
x-collection-name: Click Meter
x-complete: 0
info:
  title: Click Meter Retrieve conversion specified by id
  description: Retrieve conversion specified by id.
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /aggregated/summary/conversions:
    get:
      summary: Retrieve statistics about a subset of conversions for a timeframe with
        conversions data
      description: Retrieve statistics about a subset of conversions for a timeframe
        with conversions data.
      operationId: getAggregatedSummaryConversions
      x-api-path-slug: aggregatedsummaryconversions-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Conversions
  /conversions:
    get:
      summary: Retrieve a list of conversions
      description: Retrieve a list of conversions.
      operationId: getConversions
      x-api-path-slug: conversions-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude conversions created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude conversions created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Conversions
    post:
      summary: Create a conversion
      description: Create a conversion.
      operationId: postConversions
      x-api-path-slug: conversions-post
      parameters:
      - in: body
        name: value
        description: The body of the conversion
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
  /conversions/aggregated/list:
    get:
      summary: Retrieve statistics about this customer for a timeframe related to
        a subset of conversions grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about this customer for a timeframe related
        to a subset of conversions grouped by some temporal entity (day/week/month).
      operationId: getConversionsAggregatedList
      x-api-path-slug: conversionsaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - Aggregated
      - List
  /conversions/count:
    get:
      summary: Retrieve a count of conversions
      description: Retrieve a count of conversions.
      operationId: getConversionsCount
      x-api-path-slug: conversionscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude conversions created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude conversions created after this date (YYYYMMDD)
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - Count
  /conversions/{conversionId}:
    delete:
      summary: Delete conversion specified by id
      description: Delete conversion specified by id.
      operationId: deleteConversionsConversion
      x-api-path-slug: conversionsconversionid-delete
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
    get:
      summary: Retrieve conversion specified by id
      description: Retrieve conversion specified by id.
      operationId: getConversionsConversion
      x-api-path-slug: conversionsconversionid-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
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