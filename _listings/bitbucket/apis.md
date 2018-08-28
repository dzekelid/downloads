---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Downloads
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Get Repositories Username Repo Slug Downloads
  x-api-slug: repositoriesusernamerepo-slugdownloads-get
  description: Returns a list of download links associated with the repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Downloads
  x-api-slug: repositoriesusernamerepo-slugdownloads-parameters
  description: Parameters repositories username repo slug downloads
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Downloads
  x-api-slug: repositoriesusernamerepo-slugdownloads-post
  description: |-
    Upload new download artifacts.

    To upload files, perform a `multipart/form-data` POST containing one
    or more `files` fields:

        $ echo Hello World > hello.txt
        $ curl -s -u evzijst -X POST https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads -F files=@hello.txt

    When a file is uploaded with the same name as an existing artifact,
    then the existing file will be replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-delete
  description: Deletes the specified download artifact from the repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-get
  description: |-
    Return a redirect to the contents of a download artifact.

    This endpoint returns the actual file contents and not the artifact's
    metadata.

        $ curl -s -L https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads/hello.txt
        Hello World
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-parameters
  description: Parameters repositories username repo slug downloads filename
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---