swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
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