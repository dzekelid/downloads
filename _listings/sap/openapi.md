swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
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
  /partsAnalysis/worklists/{worklistId}/parts/{partId}/designFiles/{designFileId}:
    get:
      summary: Downloads the design file of a part
      description: Downloads the design file for a part
      operationId: downloads-the-design-file-for-a-part
      x-api-path-slug: partsanalysisworklistsworklistidpartspartiddesignfilesdesignfileid-get
      parameters:
      - in: path
        name: designFileId
        description: A self-generated ID for a design file
      - in: path
        name: partId
        description: A self-generated ID for a part in the worklist
      - in: path
        name: worklistId
        description: The UUID for a published worklist
      responses:
        200:
          description: Successful response
      tags:
      - Downloads
      - Design
      - File
      - Of
      - Part