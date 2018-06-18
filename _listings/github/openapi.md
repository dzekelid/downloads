---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  description: github-is-the-best-place-to-share-code-with-friends-coworkers-classmates-and-complete-strangers--over-24-million-people-use-github-to-build-amazing-things-together-across-67-million-repositories--with-the-collaborative-features-of-github-com-and-github-business-it-has-never-been-easier-for-individuals-and-teams-to-write-faster-better-code-
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/downloads:
    get:
      summary: Get Repos Owner Repo Downloads
      description: Deprecated. List downloads for a repository.
      operationId: deprecated-list-downloads-for-a-repository
      x-api-path-slug: reposownerrepodownloads-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Downloads
  /repos/{owner}/{repo}/downloads/{downloadId}:
    delete:
      summary: Delete Repos Owner Repo Downloads Download
      description: Deprecated. Delete a download.
      operationId: deprecated-delete-a-download
      x-api-path-slug: reposownerrepodownloadsdownloadid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: downloadId
        description: Id of download
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Downloads
      - Download
    get:
      summary: Get Repos Owner Repo Downloads Download
      description: Deprecated. Get a single download.
      operationId: deprecated-get-a-single-download
      x-api-path-slug: reposownerrepodownloadsdownloadid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: downloadId
        description: Id of download
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Downloads
      - Download
---