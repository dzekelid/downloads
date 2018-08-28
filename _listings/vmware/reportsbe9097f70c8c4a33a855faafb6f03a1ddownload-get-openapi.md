---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Download Report
  description: 'TODO: Add Description'
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/be9097f7-0c8c-4a33-a855-faafb6f03a1d/download:
    get:
      summary: Download Report
      description: 'TODO: Add Description'
      operationId: ReportsBe9097f70c8c4a33A855Faafb6f03a1dDownloadGet
      x-api-path-slug: reportsbe9097f70c8c4a33a855faafb6f03a1ddownload-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: format
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ""
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