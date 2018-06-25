---
name: Click Meter
x-slug: click-meter
description: ClickMeter was founded in 2012 as a byproduct of an experienced web-marketing
  agency. The ClickMeter System was initially a web tool created to address the needs
  of our agency to precisely count and track the web-marketing actions we performed
  for our customers.The system evolved rapidly, and emerged as one of the most widely
  used software solutions in our agency to collect, analyze, and share data for and
  with our customers. After few years after the development of the first ClickMeter
  system, we decided to go live with a service that can be useful to everyone involved
  in web-marketing activities.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Conversions
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/apis.md
specificationVersion: "0.14"
apis:
- name: Click Meter Retrieve statistics about a subset of conversions for a timeframe
    with conversions data
  x-api-slug: click-meter
  description: Retrieve statistics about a subset of conversions for a timeframe with
    conversions data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////aggregated/summary/conversions
  tags: Aggregated,Summary,Conversions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/aggregatedsummaryconversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/aggregatedsummaryconversions-get-openapi.md
- name: Click Meter Retrieve a list of conversions
  x-api-slug: click-meter
  description: Retrieve a list of conversions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions
  tags: Conversions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversions-get-openapi.md
- name: Click Meter Create a conversion
  x-api-slug: click-meter
  description: Create a conversion.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions
  tags: Conversions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversions-post-openapi.md
- name: Click Meter Retrieve statistics about this customer for a timeframe related
    to a subset of conversions grouped by some temporal entity (day/week/month)
  x-api-slug: click-meter
  description: Retrieve statistics about this customer for a timeframe related to
    a subset of conversions grouped by some temporal entity (day/week/month).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/aggregated/list
  tags: Conversions,Aggregated,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsaggregatedlist-get-openapi.md
- name: Click Meter Retrieve a count of conversions
  x-api-slug: click-meter
  description: Retrieve a count of conversions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/count
  tags: Conversions,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionscount-get-openapi.md
- name: Click Meter Delete conversion specified by id
  x-api-slug: click-meter
  description: Delete conversion specified by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}
  tags: Conversions,ConversionId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionid-delete-openapi.md
- name: Click Meter Retrieve conversion specified by id
  x-api-slug: click-meter
  description: Retrieve conversion specified by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}
  tags: Conversions,ConversionId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionid-get-openapi.md
- name: Click Meter Update conversion specified by id
  x-api-slug: click-meter
  description: Update conversion specified by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}
  tags: Conversions,ConversionId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionid-post-openapi.md
- name: Click Meter Retrieve statistics about this conversion for a timeframe
  x-api-slug: click-meter
  description: Retrieve statistics about this conversion for a timeframe.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/aggregated
  tags: Conversions,ConversionId,Aggregated
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionidaggregated-get-openapi.md
- name: Click Meter Retrieve statistics about this conversion for a timeframe grouped
    by some temporal entity (day/week/month)
  x-api-slug: click-meter
  description: Retrieve statistics about this conversion for a timeframe grouped by
    some temporal entity (day/week/month).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/aggregated/list
  tags: Conversions,ConversionId,Aggregated,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionidaggregatedlist-get-openapi.md
- name: Click Meter Retrieve a list of datapoints connected to this conversion
  x-api-slug: click-meter
  description: Retrieve a list of datapoints connected to this conversion.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/datapoints
  tags: Conversions,ConversionId,Datapoints
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversioniddatapoints-get-openapi.md
- name: Click Meter Modify the association between a conversion and multiple datapoints
  x-api-slug: click-meter
  description: Modify the association between a conversion and multiple datapoints.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/datapoints/batch/patch
  tags: Conversions,ConversionId,Datapoints,Batch,Patch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversioniddatapointsbatchpatch-put-openapi.md
- name: Click Meter Retrieve a count of datapoints connected to this conversion
  x-api-slug: click-meter
  description: Retrieve a count of datapoints connected to this conversion.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/datapoints/count
  tags: Conversions,ConversionId,Datapoints,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversioniddatapointscount-get-openapi.md
- name: Click Meter Modify the association between a conversion and a datapoint
  x-api-slug: click-meter
  description: Modify the association between a conversion and a datapoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/datapoints/patch
  tags: Conversions,ConversionId,Datapoints,Patch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversioniddatapointspatch-put-openapi.md
- name: Click Meter Retrieve the list of events related to this conversion.
  x-api-slug: click-meter
  description: Retrieve the list of events related to this conversion..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/hits
  tags: Conversions,ConversionId,Hits
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionidhits-get-openapi.md
- name: Click Meter Fast patch the "notes" field of a conversion
  x-api-slug: click-meter
  description: Fast patch the "notes" field of a conversion.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/notes
  tags: Conversions,ConversionId,Notes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionidnotes-put-openapi.md
- name: Click Meter Retrieve a top report connected to this conversion
  x-api-slug: click-meter
  description: Retrieve a top report connected to this conversion.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////conversions/{conversionId}/reports
  tags: Conversions,ConversionId,Reports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/conversionsconversionidreports-get-openapi.md
- name: Click Meter
  x-api-slug: click-meter
  description: ClickMeter was founded in 2012 as a byproduct of an experienced web-marketing
    agency. The ClickMeter System was initially a web tool created to address the
    needs of our agency to precisely count and track the web-marketing actions we
    performed for our customers.The system evolved rapidly, and emerged as one of
    the most widely used software solutions in our agency to collect, analyze, and
    share data for and with our customers. After few years after the development of
    the first ClickMeter system, we decided to go live with a service that can be
    useful to everyone involved in web-marketing activities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80//
  tags: Conversions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversions/master/_listings/click-meter/openapi.md
x-common:
- type: x-blog
  url: https://blog.clickmeter.com/
- type: x-pricing
  url: http://clickmeter.com/pricing-signup
- type: x-support
  url: https://support.clickmeter.com/hc/en-us
- type: x-terms-of-service
  url: http://clickmeter.com/terms-conditions
- type: x-twitter
  url: https://twitter.com/clickmeter
- type: x-website
  url: http://clickmeter.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---