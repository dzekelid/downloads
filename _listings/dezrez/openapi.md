---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/document/{id}/download:
    get:
      summary: Download a document by its id.
      description: Download a document by its id..
      operationId: Document_DownloadAsyncByid
      x-api-path-slug: apidocumentiddownload-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Download
      - Document
      - By
      - Its
      - Id
---