---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 0
info:
  title: Getty Images Get Downloads
  description: "Returns information about a customer's previously downloaded assets.\r\n\r\nYou'll
    need an API key and access token to use this resource. Please see our [Getting
    Started](http://developers.gettyimages.com/en/getting-started.html) page for more
    information on how to sign up for an API key. \r\n \r\n\t\r\nThis endpoint requires
    being a Getty Images customer to limit your results to only assets that you have
    a license to use, \r\nyou need to also include an authorization token in the header
    of your request. \r\nPlease consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens."
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