---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 0
info:
  title: Getty Images Download an image
  description: "Use this endpoint to generate download URLs and related data for images
    you are authorized to download.\r\n\r\nMost product offerings have enforced periodic
    download limits such as monthly, weekly, and daily. When this operation executes,
    the count of allowed downloads is decremented by one for the product offering.
    Once the download limit is reached for a given product offering, no further downloads
    may be requested for that product offering until the next download period.\r\n\r\nThe
    download limit for a given download period is covered in your product agreement
    established with Getty Images.\r\n\r\nYou'll need an API key and a [Resource Owner
    Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n## Auto Downloads\r\nThe
    `auto_download` request query parameter specifies whether to automatically download
    the image.\r\n\r\nIf the `auto_download` request query parameter is set to _true_,
    the API will return an HTTP status code 303 *See Other*.\u2002Your client code
    will need to process this response and redirect to the URI specified in the *Location*
    header to enable you to automatically download the file. The redirection workflow
    follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
    Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
    the `auto_download` request query parameter is set to false, the API will return
    a HTTP status code 200, along with the URI in the response body which can be used
    to download the image. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
  version: 1.0.0
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/downloads:
    get:
      summary: Get Downloads
      description: "Returns information about a customer's previously downloaded assets.\r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key. \r\n \r\n\t\r\nThis endpoint
        requires being a Getty Images customer to limit your results to only assets
        that you have a license to use, \r\nyou need to also include an authorization
        token in the header of your request. \r\nPlease consult our [Authorization
        FAQ](http://developers.gettyimages.com/en/authorization-faq.html) for more
        information on authorization tokens."
      operationId: Downloads_GetDownloads
      x-api-path-slug: v3downloads-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: company_downloads
        description: If specified, returns the list of previously downloaded images
          for all users in your company
      - in: query
        name: end_date
        description: If specified, select assets downloaded on or before this date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: product_type
        description: Specifies product type to be included in the previous download
          results
      - in: query
        name: start_date
        description: If specified, select assets downloaded on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
  /v3/downloads/images/{id}:
    post:
      summary: Download an image
      description: "Use this endpoint to generate download URLs and related data for
        images you are authorized to download.\r\n\r\nMost product offerings have
        enforced periodic download limits such as monthly, weekly, and daily. When
        this operation executes, the count of allowed downloads is decremented by
        one for the product offering. Once the download limit is reached for a given
        product offering, no further downloads may be requested for that product offering
        until the next download period.\r\n\r\nThe download limit for a given download
        period is covered in your product agreement established with Getty Images.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n## Auto
        Downloads\r\nThe `auto_download` request query parameter specifies whether
        to automatically download the image.\r\n\r\nIf the `auto_download` request
        query parameter is set to _true_, the API will return an HTTP status code
        303 *See Other*.\u2002Your client code will need to process this response
        and redirect to the URI specified in the *Location* header to enable you to
        automatically download the file. The redirection workflow follows the [HTTP
        1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
        Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
        the `auto_download` request query parameter is set to false, the API will
        return a HTTP status code 200, along with the URI in the response body which
        can be used to download the image. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
      operationId: Downloads_PostDownloads
      x-api-path-slug: v3downloadsimagesid-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the image
      - in: body
        name: download_details
        description: Additional information required from specific customers when
          downloading
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: file_type
        description: File Type expressed with three character file extension
      - in: query
        name: height
        description: Specifies the pixel height of the particular image to download
      - in: path
        name: id
        description: Id of image to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: product_type
        description: Product type
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
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