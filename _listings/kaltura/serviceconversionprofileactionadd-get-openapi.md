---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Conversionprofile Action Add
  description: Add new Conversion Profile
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/conversionprofile/action/add:
    get:
      summary: Get Service Conversionprofile Action Add
      description: Add new Conversion Profile
      operationId: conversionProfile.add
      x-api-path-slug: serviceconversionprofileactionadd-get
      parameters:
      - in: query
        name: conversionProfile[cropDimensions][height]
        description: Crop height
      - in: query
        name: conversionProfile[cropDimensions][left]
        description: Crop left point
      - in: query
        name: conversionProfile[cropDimensions][top]
        description: Crop top point
      - in: query
        name: conversionProfile[cropDimensions][width]
        description: Crop width
      - in: query
        name: conversionProfile[defaultEntryId]
        description: ID of the default entry to be used for template data
      - in: query
        name: conversionProfile[description]
        description: The description of the Conversion Profile
      - in: query
        name: conversionProfile[flavorParamsIds]
        description: List of included flavor ids (comma separated)
      - in: query
        name: conversionProfile[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that this conversion
          profile is system default'
      - in: query
        name: conversionProfile[name]
        description: The name of the Conversion Profile
      - in: query
        name: conversionProfile[status]
        description: 'Enum Type: `KalturaConversionProfileStatus`'
      - in: query
        name: conversionProfile[systemName]
        description: System name of the Conversion Profile
      - in: query
        name: conversionProfile[tags]
        description: Comma separated tags
      - in: query
        name: conversionProfile[type]
        description: '`insertOnly`Enum Type: `KalturaConversionProfileType`'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
      - Action
      - Add
  /service/conversionprofile/action/delete:
    get:
      summary: Get Service Conversionprofile Action Delete
      description: Delete Conversion Profile by ID
      operationId: conversionProfile.delete
      x-api-path-slug: serviceconversionprofileactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
      - Action
      - Delete
  /service/conversionprofile/action/get:
    get:
      summary: Get Service Conversionprofile Action Get
      description: Get Conversion Profile by ID
      operationId: conversionProfile.get
      x-api-path-slug: serviceconversionprofileactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
      - Action
      - Get
  /service/conversionprofile/action/getDefault:
    get:
      summary: Get Service Conversionprofile Action Getdefault
      description: Get the partner's default conversion profile
      operationId: conversionProfile.getDefault
      x-api-path-slug: serviceconversionprofileactiongetdefault-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: type
        description: 'Enum Type: `KalturaConversionProfileType`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
      - Action
      - GetDefault
  /service/conversionprofile/action/list:
    get:
      summary: Get Service Conversionprofile Action List
      description: List Conversion Profiles by filter with paging support
      operationId: conversionProfile.list
      x-api-path-slug: serviceconversionprofileactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[defaultEntryIdEqual]
      - in: query
        name: filter[defaultEntryIdIn]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[nameEqual]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaConversionProfileStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaConversionProfileType`'
      - in: query
        name: filter[typeIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
      - Action
      - List
  /service/conversionprofile/action/setAsDefault:
    get:
      summary: Get Service Conversionprofile Action Setasdefault
      description: Set Conversion Profile to be the partner default
      operationId: conversionProfile.setAsDefault
      x-api-path-slug: serviceconversionprofileactionsetasdefault-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
      - Action
      - SetAsDefault
  /service/conversionprofile/action/update:
    get:
      summary: Get Service Conversionprofile Action Update
      description: Update Conversion Profile by ID
      operationId: conversionProfile.update
      x-api-path-slug: serviceconversionprofileactionupdate-get
      parameters:
      - in: query
        name: conversionProfile[cropDimensions][height]
        description: Crop height
      - in: query
        name: conversionProfile[cropDimensions][left]
        description: Crop left point
      - in: query
        name: conversionProfile[cropDimensions][top]
        description: Crop top point
      - in: query
        name: conversionProfile[cropDimensions][width]
        description: Crop width
      - in: query
        name: conversionProfile[defaultEntryId]
        description: ID of the default entry to be used for template data
      - in: query
        name: conversionProfile[description]
        description: The description of the Conversion Profile
      - in: query
        name: conversionProfile[flavorParamsIds]
        description: List of included flavor ids (comma separated)
      - in: query
        name: conversionProfile[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that this conversion
          profile is system default'
      - in: query
        name: conversionProfile[name]
        description: The name of the Conversion Profile
      - in: query
        name: conversionProfile[status]
        description: 'Enum Type: `KalturaConversionProfileStatus`'
      - in: query
        name: conversionProfile[systemName]
        description: System name of the Conversion Profile
      - in: query
        name: conversionProfile[tags]
        description: Comma separated tags
      - in: query
        name: conversionProfile[type]
        description: '`insertOnly`Enum Type: `KalturaConversionProfileType`'
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofile
      - Action
      - Update
  /service/conversionprofileassetparams/action/list:
    get:
      summary: Get Service Conversionprofileassetparams Action List
      description: Lists asset parmas of conversion profile by ID
      operationId: conversionProfileAssetParams.list
      x-api-path-slug: serviceconversionprofileassetparamsactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[assetParamsIdEqual]
      - in: query
        name: filter[assetParamsIdIn]
      - in: query
        name: filter[conversionProfileIdEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][categoryIdEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][contentLike]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][distributionProfileId]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][extendedStatusIn]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][field]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][idEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][idIn]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][items]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][memberIdEq]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][memberIdIn]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][metadataProfileId]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][not]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][objectType]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][userIdEqual]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][userIdIn]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][value]
      - in: query
        name: filter[conversionProfileIdFilter][advancedSearch][watermarkId]
      - in: query
        name: filter[conversionProfileIdFilter][defaultEntryIdEqual]
      - in: query
        name: filter[conversionProfileIdFilter][defaultEntryIdIn]
      - in: query
        name: filter[conversionProfileIdFilter][idEqual]
      - in: query
        name: filter[conversionProfileIdFilter][idIn]
      - in: query
        name: filter[conversionProfileIdFilter][nameEqual]
      - in: query
        name: filter[conversionProfileIdFilter][orderBy]
      - in: query
        name: filter[conversionProfileIdFilter][statusEqual]
        description: 'Enum Type: `KalturaConversionProfileStatus`'
      - in: query
        name: filter[conversionProfileIdFilter][statusIn]
      - in: query
        name: filter[conversionProfileIdFilter][systemNameEqual]
      - in: query
        name: filter[conversionProfileIdFilter][systemNameIn]
      - in: query
        name: filter[conversionProfileIdFilter][tagsMultiLikeAnd]
      - in: query
        name: filter[conversionProfileIdFilter][tagsMultiLikeOr]
      - in: query
        name: filter[conversionProfileIdFilter][typeEqual]
        description: 'Enum Type: `KalturaConversionProfileType`'
      - in: query
        name: filter[conversionProfileIdFilter][typeIn]
      - in: query
        name: filter[conversionProfileIdIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[originEqual]
        description: 'Enum Type: `KalturaAssetParamsOrigin`'
      - in: query
        name: filter[originIn]
      - in: query
        name: filter[readyBehaviorEqual]
        description: 'Enum Type: `KalturaFlavorReadyBehaviorType`'
      - in: query
        name: filter[readyBehaviorIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofileassetparams
      - Action
      - List
  /service/conversionprofileassetparams/action/update:
    get:
      summary: Get Service Conversionprofileassetparams Action Update
      description: Update asset parmas of conversion profile by ID
      operationId: conversionProfileAssetParams.update
      x-api-path-slug: serviceconversionprofileassetparamsactionupdate-get
      parameters:
      - in: query
        name: assetParamsId
      - in: query
        name: conversionProfileAssetParams[contentAwareness]
      - in: query
        name: conversionProfileAssetParams[deletePolicy]
        description: 'Enum Type: `KalturaAssetParamsDeletePolicy`Specifies how to
          treat the flavor after conversion is finished'
      - in: query
        name: conversionProfileAssetParams[forceNoneComplied]
        description: 'Enum Type: `KalturaNullableBoolean`Starts conversion even if
          the decision layer reduced the configuration to comply with the source'
      - in: query
        name: conversionProfileAssetParams[isEncrypted]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: conversionProfileAssetParams[origin]
        description: 'Enum Type: `KalturaAssetParamsOrigin`The ingestion origin of
          the asset params'
      - in: query
        name: conversionProfileAssetParams[readyBehavior]
        description: 'Enum Type: `KalturaFlavorReadyBehaviorType`The ingestion origin
          of the asset params'
      - in: query
        name: conversionProfileAssetParams[systemName]
        description: Asset params system name
      - in: query
        name: conversionProfileAssetParams[tags]
      - in: query
        name: conversionProfileAssetParams[twoPass]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: conversionProfileId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Conversionprofileassetparams
      - Action
      - Update
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