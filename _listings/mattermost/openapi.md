swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels/{channel_id}/convert:
    post:
      summary: Convert a channel from public to private
      description: |-
        Convert into private channel from the provided channel id string.

        __Minimum server version__: 4.10

        ##### Permissions
        Must have `manage_system` permission.
      operationId: convert-into-private-channel-from-the-provided-channel-id-string-minimum-server-version--410-permiss
      x-api-path-slug: channelschannel-idconvert-post
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Convert
      - Channel
      - From
      - Public
      - To
      - Private