---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{id}/download:
    post:
      summary: Download the latest translation package.
      description: Download the latest translation package. You must have given a
        /package call beforehand and wait until the packaging status is 'completed'.
      operationId: download
      x-api-path-slug: projectsiddownload-post
      parameters:
      - in: path
        name: id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Download
  /projects/{id}/download/{language}:
    post:
      summary: Download the latest translation package.
      description: Download only the translation package of this language. You must
        have given a /package call beforehand and wait until the packaging status
        is 'completed'.
      operationId: downloadLanguage
      x-api-path-slug: projectsiddownloadlanguage-post
      parameters:
      - in: path
        name: id
        description: Project ID
      - in: path
        name: language
        description: Language code
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Download
      - Language
  /projects/{projectId}/documents/{documentId}/download:
    get:
      summary: Download a document
      description: Download a document.
      operationId: downloadDocument
      x-api-path-slug: projectsprojectiddocumentsdocumentiddownload-get
      parameters:
      - in: path
        name: documentId
        description: Document ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Documents
      - DocumentId
      - Download
  /projects/{projectId}/glossaries/{glossaryId}/download:
    get:
      summary: Download a glossary
      description: Download a glossary.
      operationId: downloadGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryiddownload-get
      parameters:
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
      - Download
  /projects/{projectId}/styleguides/{styleGuideId}/download:
    get:
      summary: Download a style guide
      description: Download a style guide.
      operationId: downloadStyleGuide
      x-api-path-slug: projectsprojectidstyleguidesstyleguideiddownload-get
      parameters:
      - in: path
        name: projectId
        description: Project ID
      - in: path
        name: styleGuideId
        description: Style Guide ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Styleguides
      - StyleGuideId
      - Download
---