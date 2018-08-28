---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Download a report
  description: |-
    Download the full contents of a report as a file.
    ##### Permissions
    Must have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /compliance/reports/{report_id}/download:
    get:
      summary: Download a report
      description: |-
        Download the full contents of a report as a file.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: download-the-full-contents-of-a-report-as-a-file-permissionsmust-have-manage-system-permission
      x-api-path-slug: compliancereportsreport-iddownload-get
      parameters:
      - in: path
        name: report_id
        description: Compliance report GUID
      responses:
        200:
          description: OK
      tags:
      - Download
      - Report
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