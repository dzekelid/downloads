---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Download Media
  description: Download a Media file from the Library
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /library/download/{mediaId}/{type}:
    get:
      summary: Download Media
      description: Download a Media file from the Library
      operationId: libraryDownload
      x-api-path-slug: librarydownloadmediaidtype-get
      parameters:
      - in: path
        name: mediaId
        description: The Media ID to Download
      - in: path
        name: type
        description: The Module Type of the Download
      responses:
        200:
          description: OK
      tags:
      - Download
      - Media
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