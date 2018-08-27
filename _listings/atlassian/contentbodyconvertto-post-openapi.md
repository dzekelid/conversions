---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Convert content body
  description: |-
    Converts a content body from one format to another format.

    Supported conversions:

    - storage: view, export_view, styled_view, editor
    - editor: storage
    - view: none
    - export_view: none
    - styled_view: none

    **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    If request specifies 'contentIdContext', 'View' permission for the space, and permission to view the content.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contentbody/convert/{to}:
    post:
      summary: Convert content body
      description: |-
        Converts a content body from one format to another format.

        Supported conversions:

        - storage: view, export_view, styled_view, editor
        - editor: storage
        - view: none
        - export_view: none
        - styled_view: none

        **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
        If request specifies 'contentIdContext', 'View' permission for the space, and permission to view the content.
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentBodyResource.convertContentBody_post
      x-api-path-slug: contentbodyconvertto-post
      parameters:
      - in: query
        name: contentIdContext
        description: The content ID used to find the space for resolving embedded
          content (page includes, files, and links) in the content body
      - in: query
        name: embeddedContentRender
        description: Mode used for rendering embedded content, like attachments
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the new
          content to expand
      - in: query
        name: spaceKeyContext
        description: The space key used for resolving embedded content (page includes,
          files, and links) in the content body
      - in: path
        name: to
        description: The name of the target format for the content body
      responses:
        200:
          description: OK
      tags:
      - Convert
      - Content
      - Body
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