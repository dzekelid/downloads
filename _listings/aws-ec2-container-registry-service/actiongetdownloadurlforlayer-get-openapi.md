---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Get Download Url For Layer
  version: 1.0.0
  description: .Retrieves the pre-signed Amazon S3 download URL corresponding to an
    image layer. You can only get URLs for image layers that are referenced in an
    image.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDownloadUrlForLayer:
    get:
      summary: Get Download Url For Layer
      description: .Retrieves the pre-signed Amazon S3 download URL corresponding
        to an image layer. You can only get URLs for image layers that are referenced
        in an image.
      operationId: getDownloadUrlForLayer
      x-api-path-slug: actiongetdownloadurlforlayer-get
      responses:
        200:
          description: OK
      tags:
      - Layers
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