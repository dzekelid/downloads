---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Download The Contents Of A Drive Item
  description: Download the contents of a DriveItem Download the contents for a driveItem.
    Only driveItem with the file property can be downloaded.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/drive/root:/{item-path}:/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: medriverootitempathcontent-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
  /me/drive/items/{item-id}/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: medriveitemsitemidcontent-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
  /drives/items/{item-id}/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: drivesitemsitemidcontent-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
  /groups/{group-id}/drive/items/{item-id}/content:
    get:
      summary: Download The Contents Of A Drive Item
      description: Download the contents of a DriveItem Download the contents for
        a driveItem. Only driveItem with the file property can be downloaded.
      operationId: DownloadTheContentsOfADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidcontent-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - DownloadContents
      - OfDrive
      - Item
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