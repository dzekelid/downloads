swagger: "2.0"
x-collection-name: Fluxiom
x-complete: 1
info:
  title: Fluxiom API
  description: the-fluxiom-api-allows-you-to-hook-into-fluxiom-and-connect-it-with-other-apps-
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