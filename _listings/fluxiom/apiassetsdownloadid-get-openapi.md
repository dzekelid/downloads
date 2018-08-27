---
swagger: "2.0"
x-collection-name: Fluxiom
x-complete: 0
info:
  title: Fluxiom API Download asset
  description: Download asset
  termsOfService: http://www.fluxiom.com/terms
  version: v1
host: '{subdomain}.fluxiom.com'
basePath: /api/{format}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/assets/download/{id}:
    get:
      summary: Download asset
      description: Download asset
      operationId: download-asset
      x-api-path-slug: apiassetsdownloadid-get
      parameters:
      - in: path
        name: ID
        description: The unique ID for the asset
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Download
      - Id
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