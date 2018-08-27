swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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