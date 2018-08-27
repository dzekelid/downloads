---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Post App Content Product Download
  description: Returns a temporary URL where the client can download the content.
    In the payload, the receipt string is the receipt data from the purchase. It should
    be unaltered from how Apple delivers it to your application.udid is an optional
    field to help identify a particular user???s purchases, which can aid debugging.
    It should always be a hash of the UDID, not the actual UDID, to ensure compliance
    with Apple???s TOS. The optional version field should be the StoreFront library
    version, or custom if you???re building your own.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /app/content/{product_id}/download:
    post:
      summary: Post App Content Product Download
      description: Returns a temporary URL where the client can download the content.
        In the payload, the receipt string is the receipt data from the purchase.
        It should be unaltered from how Apple delivers it to your application.udid
        is an optional field to help identify a particular user???s purchases, which
        can aid debugging. It should always be a hash of the UDID, not the actual
        UDID, to ensure compliance with Apple???s TOS. The optional version field
        should be the StoreFront library version, or custom if you???re building your
        own.
      operationId: app.content.product_id.download.post
      x-api-path-slug: appcontentproduct-iddownload-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: product_id
        description: The product ID
      - in: path
        name: product_id
      responses:
        200:
          description: OK
      tags:
      - App
      - Content
      - Product
      - Id
      - Download
  /user/{user_id}/subscriptions/content/{content_id}/download:
    post:
      summary: Post User User Subscriptions Content Content Download
      description: Downloads the content.
      operationId: user.user_id.subscriptions.content.content_id.download.post
      x-api-path-slug: useruser-idsubscriptionscontentcontent-iddownload-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: content_id
        description: Content ID
      - in: path
        name: content_id
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Subscriptions
      - Content
      - Content
      - Id
      - Download
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