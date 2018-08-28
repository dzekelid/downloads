---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Starts download of signed contract document
  description: Starts download of signed contract document.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/categories/{categoryId}/documents/downloads:
    get:
      summary: Download category documents
      description: Downloads the documents of a category as a zip file. The ID of
        the category must be specified.
      operationId: getRestCategoriesCategoryDocumentsDownloads
      x-api-path-slug: restcategoriescategoryiddocumentsdownloads-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Category
      - Documents
  /rest/customer_contracts/{contractId}/document:
    get:
      summary: Starts download of contract document
      description: Starts download of contract document.
      operationId: getRestCustomerContractsContractDocument
      x-api-path-slug: restcustomer-contractscontractiddocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Contract
      - Document
  /rest/customer_contracts/{contractId}/sign/document:
    get:
      summary: Starts download of signed contract document
      description: Starts download of signed contract document.
      operationId: getRestCustomerContractsContractSignDocument
      x-api-path-slug: restcustomer-contractscontractidsigndocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Signed
      - Contract
      - Document
  /rest/documents/{documentId}:
    get:
      summary: Download the content of a document
      description: Downloads the content of a document. The ID of the document must
        be specified.
      operationId: getRestDocumentsDocument
      x-api-path-slug: restdocumentsdocumentid-get
      parameters:
      - in: path
        name: documentId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Content
      - Of
      - Document
  /rest/orders/documents/downloads/{type}:
    get:
      summary: Download documents of a document type
      description: Downloads documents of the same document type as a zip file. The
        type of the documents must be specified.
      operationId: getRestOrdersDocumentsDownloadsType
      x-api-path-slug: restordersdocumentsdownloadstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: query
        name: itemsPerPage
        description: The number of documents to display per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: plentyId
        description: The plenty ID of the order documents
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Download
      - Documents
      - Of
      - Document
      - Type
  /rest/orders/{orderId}/documents/downloads/{type?}:
    get:
      summary: Download documents of an order
      description: Downloads documents of an order as a zip file. The ID of the order
        must be specified. In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsDownloadsType
      x-api-path-slug: restordersorderiddocumentsdownloadstype-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the document
      - in: path
        name: type?
      responses:
        200:
          description: OK
      tags:
      - Download
      - Documents
      - Of
      - Order
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