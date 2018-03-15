---
swagger: "2.0"
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /agency/{agencyId}/advertiser/{advertiserId}/engine/{engineAccountId}/conversion:
    get:
      summary: Get Conversions
      description: Retrieves a list of conversions from a DoubleClick Search engine
        account
      operationId: doubleclicksearch.conversion.get
      parameters:
      - in: query
        name: adGroupId
        description: Numeric ID of the ad group
      - in: query
        name: adId
        description: Numeric ID of the ad
      - in: path
        name: advertiserId
        description: Numeric ID of the advertiser
      - in: path
        name: agencyId
        description: Numeric ID of the agency
      - in: query
        name: campaignId
        description: Numeric ID of the campaign
      - in: query
        name: criterionId
        description: Numeric ID of the criterion
      - in: query
        name: endDate
        description: Last date (inclusive) on which to retrieve conversions
      - in: path
        name: engineAccountId
        description: Numeric ID of the engine account
      - in: query
        name: rowCount
        description: The number of conversions to return per call
      - in: query
        name: startDate
        description: First date (inclusive) on which to retrieve conversions
      - in: query
        name: startRow
        description: The 0-based starting index for retrieving conversions results
      responses:
        200:
          description: OK
      tags:
      - advertising
      - conversion
definitions: []
x-collection-name: Google Doubleclick
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