---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToAssist Remote Support Download Recordings
  description: "This method retrieves download links for a list of recordings. Each
    recording returns a link to the MP4 file, the .events file and the thumbnail.
    If a recording is not available for download then it will be omitted from the
    returned list. The archiving script may use the returned URLs to download each
    resource for the recording. The URLs will be valid for at least 48 hours. The
    URL contains a large random number so that the URL for recordings cannot be guessed.
    The response includes the recording start time to make it easier for the archiving
    script to place recordings in directories based on date. No more than 500 recordings
    can be requested at once.\n\nNote: Session recording must be enabled on the account
    in order to use this API method. To enable session recording, log in at https://app.gotoassist.com
    (link is external) and go to Configure > GoToAssist Settings > Enable Session
    Recording check box.\n\n  Response Parameters                  \n                    \n
    \   field      data type      description    \n    recordingId      number      The
    recordingId of the session recording to be downloaded    \n    recordingUrl      string
    \     The URL of MP4 recording file    \n    recordingStartTime      ISO 8601
    format*      The start time of recording    \n    eventsUrl      string      The
    URL of the events recording file    \n    thumbnailUrl      string      The URL
    of the thumbnail of recording file    \n    recordingSize      string      The
    size of the .mp4 file in bytes    \n\n* ISO 8601 format reference\n                    \nStatus
    Codes                    \n                    \n    Staus Code      description
    \         \n    200 OK      A list of URLs has been returned          \n    400
    Bad Request      Request may be malformed or property may be missing or invalid
    \         \n    403 Forbidden      Invalid authorization header or invalid recording
    Ids          \n    500 Internal Server Error      Unexpected server error"
  version: 1.0.0
host: api.getgo.com
basePath: /G2A/rest/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /archive/recordings/urls[&{attribute}={readyForDownloadRecordingId}]:
    get:
      summary: Download Recordings
      description: "This method retrieves download links for a list of recordings.
        Each recording returns a link to the MP4 file, the .events file and the thumbnail.
        If a recording is not available for download then it will be omitted from
        the returned list. The archiving script may use the returned URLs to download
        each resource for the recording. The URLs will be valid for at least 48 hours.
        The URL contains a large random number so that the URL for recordings cannot
        be guessed. The response includes the recording start time to make it easier
        for the archiving script to place recordings in directories based on date.
        No more than 500 recordings can be requested at once.\n\nNote: Session recording
        must be enabled on the account in order to use this API method. To enable
        session recording, log in at https://app.gotoassist.com (link is external)
        and go to Configure > GoToAssist Settings > Enable Session Recording check
        box.\n\n  Response Parameters                  \n                    \n    field
        \     data type      description    \n    recordingId      number      The
        recordingId of the session recording to be downloaded    \n    recordingUrl
        \     string      The URL of MP4 recording file    \n    recordingStartTime
        \     ISO 8601 format*      The start time of recording    \n    eventsUrl
        \     string      The URL of the events recording file    \n    thumbnailUrl
        \     string      The URL of the thumbnail of recording file    \n    recordingSize
        \     string      The size of the .mp4 file in bytes    \n\n* ISO 8601 format
        reference\n                    \nStatus Codes                    \n                    \n
        \   Staus Code      description          \n    200 OK      A list of URLs
        has been returned          \n    400 Bad Request      Request may be malformed
        or property may be missing or invalid          \n    403 Forbidden      Invalid
        authorization header or invalid recording Ids          \n    500 Internal
        Server Error      Unexpected server error"
      operationId: ArchiveRecordingsUrlsAPIGet
      x-api-path-slug: archiverecordingsurlsattributereadyfordownloadrecordingid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: attribute
      - in: header
        name: Content-Type
      - in: path
        name: readyForDownloadRecordingId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Recordings
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