---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
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
  /userprofiles/{profileId}/conversions/batchinsert:
    post:
      summary: Insert Conversions
      description: Inserts conversions.
      operationId: dfareporting.conversions.batchinsert
      x-api-path-slug: userprofilesprofileidconversionsbatchinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
  /agency/{agencyId}/advertiser/{advertiserId}/engine/{engineAccountId}/conversion:
    get:
      summary: Get Conversions
      description: Retrieves a list of conversions from a DoubleClick Search engine
        account.
      operationId: doubleclicksearch.conversion.get
      x-api-path-slug: agencyagencyidadvertiseradvertiseridengineengineaccountidconversion-get
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
      - Advertising
      - Conversion
  /conversion:
    patch:
      summary: Update Conversions
      description: Updates a batch of conversions in DoubleClick Search. This method
        supports patch semantics.
      operationId: doubleclicksearch.conversion.patch
      x-api-path-slug: conversion-patch
      parameters:
      - in: query
        name: advertiserId
        description: Numeric ID of the advertiser
      - in: query
        name: agencyId
        description: Numeric ID of the agency
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: endDate
        description: Last date (inclusive) on which to retrieve conversions
      - in: query
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
      - Advertising
      - Conversion
    post:
      summary: Insert Conversion
      description: Inserts a batch of new conversions into DoubleClick Search.
      operationId: doubleclicksearch.conversion.insert
      x-api-path-slug: conversion-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
    put:
      summary: Update Conversions
      description: Updates a batch of conversions in DoubleClick Search.
      operationId: doubleclicksearch.conversion.update
      x-api-path-slug: conversion-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
  /conversion/updateAvailability:
    post:
      summary: Update Availability
      description: Updates the availabilities of a batch of floodlight activities
        in DoubleClick Search.
      operationId: doubleclicksearch.conversion.updateAvailability
      x-api-path-slug: conversionupdateavailability-post
      parameters:
      - in: body
        name: empty
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
---