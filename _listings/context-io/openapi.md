swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/files/{fileId}/content:
    get:
      summary: Get Accounts Files Fileid Content
      description: 'Downloads a given file. Returns the content a given attachment.
        On-demand data retrieval: since we do not keep full copies of attachments
        on our servers, the file has to be retrieved from the IMAP server when this
        call is made. If the IMAP server is unreachable at the time the call is made,
        this call will return an error.'
      operationId: getAccountFileContent_
      x-api-path-slug: accountsidfilesfileidcontent-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Content