swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
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