---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DownloadDBLogFilePortion:
    get:
      summary: Download D B Log File Portion
      description: Downloads all or a portion of the specified log file, up to 1 MB
        in size.
      operationId: downloaddblogfileportion
      x-api-path-slug: actiondownloaddblogfileportion-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The customer-assigned name of the DB instance that contains the
          log files you want to list
        type: string
      - in: query
        name: LogFileName
        description: The name of the log file to be downloaded
        type: string
      - in: query
        name: Marker
        description: The pagination token provided in the previous request or 0
        type: string
      - in: query
        name: NumberOfLines
        description: The number of lines to download
        type: string
      responses:
        200:
          description: OK
      tags:
      - Log Files
---