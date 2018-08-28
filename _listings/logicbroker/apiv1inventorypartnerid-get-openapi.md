---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Download inventory as CSV.
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Inventory/{partnerId}:
    get:
      summary: Download inventory as CSV.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Inventory_Download
      x-api-path-slug: apiv1inventorypartnerid-get
      parameters:
      - in: query
        name: fileType
        description: CSV or XLSX
      - in: query
        name: includeNullQuantity
        description: Set to true to include items with null quantity
      - in: query
        name: mapped
        description: Set to false to view items with no merchant SKU
      - in: query
        name: modifiedAfter
        description: Only items modified after this time
      - in: path
        name: partnerId
        description: Partner account number
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Download
      - Inventory
      - As
      - CSV
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