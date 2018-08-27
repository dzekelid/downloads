---
name: UK National Archives Discovery
x-slug: uk-national-archives-discovery
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Downloads
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/uk-national-archives-discovery/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Search API Get Downloads
  x-api-slug: getty-images-search-api
  description: Returns information about a customer's downloaded assets..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads
  tags: Downloads
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/uk-national-archives-discovery/v3downloads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/uk-national-archives-discovery/v3downloads-get-openapi.md
- name: Getty Images Search API Post Downloads Images
  x-api-slug: getty-images-search-api
  description: Download an image.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads/images/{id}
  tags: Downloads,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/uk-national-archives-discovery/v3downloadsimagesid-post-openapi.md
- name: Getty Images Search API Post Downloads Veos
  x-api-slug: getty-images-search-api
  description: Download a video.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads/videos/{id}
  tags: Downloads,Veos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/uk-national-archives-discovery/v3downloadsvideosid-post-openapi.md
- name: Getty Images Search API Post Downloads
  x-api-slug: getty-images-search-api
  description: Download an image.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads/{id}
  tags: Downloads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/uk-national-archives-discovery/v3downloadsid-post-openapi.md
- name: Getty Images Search API
  x-api-slug: getty-images-search-api
  description: Our set of APIs enable seamless integration of Getty Images expansive
    content, powerful search and rich metadata directly into your internal workflows,
    products and services. With Connects API solutions, you can fully control, customize
    and scale as you grow.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com//
  tags: Downloads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/uk-national-archives-discovery/openapi.md
x-common:
- type: x-website
  url: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
- type: x-website
  url: http:///Search
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---