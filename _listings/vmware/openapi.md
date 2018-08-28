swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
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