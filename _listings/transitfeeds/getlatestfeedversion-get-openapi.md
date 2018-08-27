---
swagger: "2.0"
x-collection-name: TransitFeeds
x-complete: 0
info:
  title: TransitFeeds Retrieve the download URL for the latest version of a feed.
  description: |-
    Once you have used `/getFeeds` to discover a feed's URL, you can use this endpoint to download its latest version from TranstiFeeds.
    It will be unmodified in the original format from the provider.
  contact:
    name: TransitFeeds.com
    url: https://transitfeeds.com/issues
    email: support@transitfeeds.com
  version: 1.0.0
host: api.transitfeeds.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getLatestFeedVersion:
    get:
      summary: Retrieve the download URL for the latest version of a feed.
      description: |-
        Once you have used `/getFeeds` to discover a feed's URL, you can use this endpoint to download its latest version from TranstiFeeds.
        It will be unmodified in the original format from the provider.
      operationId: getLatestFeedVersion
      x-api-path-slug: getlatestfeedversion-get
      parameters:
      - in: query
        name: feed
        description: The ID of the feed to retrieve the latest feed version for
      - in: query
        name: key
        description: Your personal API key, used for authentication
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Download
      - URLthe
      - Latest
      - Version
      - Of
      - Feed
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