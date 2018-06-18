---
name: Getty Images
x-slug: getty-images
description: Find high resolution royalty-free images, editorial stock photos, vector
  art, video footage clips and stock music licensing at the richest image search photo
  library online.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
x-kinRank: "8"
x-alexaRank: "1939"
tags: Downloads
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/getty-images/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Get Downloads
  x-api-slug: getty-images
  description: "Returns information about a customer's previously downloaded assets.\r\n\r\nYou'll
    need an API key and access token to use this resource. Please see our [Getting
    Started](http://developers.gettyimages.com/en/getting-started.html) page for more
    information on how to sign up for an API key. \r\n \r\n\t\r\nThis endpoint requires
    being a Getty Images customer to limit your results to only assets that you have
    a license to use, \r\nyou need to also include an authorization token in the header
    of your request. \r\nPlease consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/downloads
  tags: Images,Downloads
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/getty-images/v3downloads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/getty-images/v3downloads-get-openapi.md
- name: Getty Images Download an image
  x-api-slug: getty-images
  description: "Use this endpoint to generate download URLs and related data for images
    you are authorized to download.\r\n\r\nMost product offerings have enforced periodic
    download limits such as monthly, weekly, and daily. When this operation executes,
    the count of allowed downloads is decremented by one for the product offering.
    Once the download limit is reached for a given product offering, no further downloads
    may be requested for that product offering until the next download period.\r\n\r\nThe
    download limit for a given download period is covered in your product agreement
    established with Getty Images.\r\n\r\nYou'll need an API key and a [Resource Owner
    Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n## Auto Downloads\r\nThe
    `auto_download` request query parameter specifies whether to automatically download
    the image.\r\n\r\nIf the `auto_download` request query parameter is set to _true_,
    the API will return an HTTP status code 303 *See Other*.\u2002Your client code
    will need to process this response and redirect to the URI specified in the *Location*
    header to enable you to automatically download the file. The redirection workflow
    follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
    Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
    the `auto_download` request query parameter is set to false, the API will return
    a HTTP status code 200, along with the URI in the response body which can be used
    to download the image. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/downloads/images/{id}
  tags: Images,Downloads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/getty-images/v3downloadsimagesid-post-openapi.md
- name: Getty Images Download a video
  x-api-slug: getty-images
  description: "Use this endpoint to generate download URLs and related data for videos
    you are authorized to download.\r\n\r\nMost product offerings have enforced periodic
    download limits such as monthly, weekly, and daily. When this operation executes,
    the count of allowed downloads is decremented by one for the product offering.
    Once the download limit is reached for a given product offering, no further downloads
    may be requested for that product offering until the next download period.\r\n\r\nThe
    download limit for a given download period is covered in your product agreement
    established with Getty Images.\r\n\r\nYou'll need an API key and a [Resource Owner
    Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n## Auto Downloads\r\nThe
    `auto_download` request query parameter specifies whether to automatically download
    the video.\r\n\r\nIf the `auto_download` request query parameter is set to _true_,
    the API will return an HTTP status code 303 *See Other*.\u2002Your client code
    will need to process this response and redirect to the URI specified in the *Location*
    header to enable you to automatically download the file. The redirection workflow
    follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
    Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
    the `auto_download` request query parameter is set to false, the API will return
    a HTTP status code 200, along with the URI in the response body which can be used
    to download the video. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/downloads/videos/{id}
  tags: Images,Downloads,Videos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/getty-images/v3downloadsvideosid-post-openapi.md
- name: Getty Images
  x-api-slug: getty-images
  description: Find high resolution royalty-free images, editorial stock photos, vector
    art, video footage clips and stock music licensing at the richest image search
    photo library online.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Downloads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/downloads/master/_listings/getty-images/openapi.md
x-common:
- type: x-authentication
  url: https://github.com/gettyimages/connect#authentication
- type: x-base
  url: https://connect.gettyimages.com/
- type: x--net-sdk
  url: https://github.com/gettyimages/connect_sdk_csharp
- type: x-crunchbase
  url: https://crunchbase.com/organization/gettyimages
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ge-tt
- type: x-developer
  url: http://api.gettyimages.com/
- type: x-documentation
  url: https://api.gettyimages.com/swagger/ui/index.html
- type: x-email
  url: privacy@gettyimages.com
- type: x-email
  url: sales@gettyimages.com
- type: x-email
  url: copyright@gettyimages.com
- type: x-embeddable
  url: https://github.com/gettyimages/connect#oembed
- type: x-forum
  url: http://api.gettyimages.com/forum
- type: x-getting-started
  url: https://github.com/gettyimages/connect#getting-started
- type: x-github
  url: https://github.com/gettyimages
- type: x-java-sdk
  url: https://github.com/gettyimages/connect_sdk_java
- type: x-node-js-sdk
  url: https://github.com/gettyimages/connect_sdk_nodejs
- type: x-objectivec-sdk
  url: https://github.com/gettyimages/connect_sdk_objective-c
- type: x-php-sdk
  url: https://github.com/gettyimages/connect_sdk_php
- type: x-pricing
  url: http://www.gettyimages.com/subscribe
- type: x-ruby-sdk
  url: https://github.com/gettyimages/connect_sdk_ruby
- type: x-twitter
  url: https://twitter.com/GettyImages
- type: x-website
  url: http://www.gettyimages.com/
- type: x-website
  url: http://gettyimages.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---