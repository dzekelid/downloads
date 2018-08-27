---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 1
info:
  title: Official Akeneo PIM API
  description: the-akeneo-api-brought-to-youfind-out-how-this-postman-collection-works-by-visiting-httpapi-akeneo-com
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/assets/paint/reference-files/no-locale/download:
    get:
      summary: download asset reference file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset and an activated locale if the asset is localizable (it should be equal
        to "no-locale" otherwise)
      operationId: RestV1AssetsPaintReferenceFilesNoLocaleDownloadGet
      x-api-path-slug: restv1assetspaintreferencefilesnolocaledownload-get
      responses:
        200:
          description: OK
      tags:
      - Download
      - Asset
      - Reference
      - File
      - (2
      - "1"
      - Only)
  /rest/v1/assets/paint/variation-files/ecommerce/no-locale/download:
    get:
      summary: download asset variation file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset, an existing channel and an activated locale if the asset is localizable
        (it should be equal to "no-locale" otherwise)
      operationId: RestV1AssetsPaintVariationFilesEcommerceNoLocaleDownloadGet
      x-api-path-slug: restv1assetspaintvariationfilesecommercenolocaledownload-get
      responses:
        200:
          description: OK
      tags:
      - Download
      - Asset
      - Variation
      - File
      - (2
      - "1"
      - Only)
---