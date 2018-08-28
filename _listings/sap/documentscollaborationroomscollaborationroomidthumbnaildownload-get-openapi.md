---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Partner APIs Downloads the thumbnail of a design
    file
  description: Downloads the thumbnail selected as the icon for a collaboration room.
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /documents/collaborationRooms/{collaborationRoomId}/download:
    get:
      summary: Downloads a file
      description: Downloads a file from a collaboration room.
      operationId: downloads-a-file-from-a-collaboration-room
      x-api-path-slug: documentscollaborationroomscollaborationroomiddownload-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: query
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - Downloads
      - File
  /documents/collaborationRooms/{collaborationRoomId}/thumbnail/download:
    get:
      summary: Downloads the thumbnail of a design file
      description: Downloads the thumbnail selected as the icon for a collaboration
        room.
      operationId: downloads-the-thumbnail-selected-as-the-icon-for-a-collaboration-room
      x-api-path-slug: documentscollaborationroomscollaborationroomidthumbnaildownload-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Downloads
      - Thumbnail
      - Of
      - Design
      - File
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