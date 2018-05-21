---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get User Albums
  description: User Albums
  termsOfService: https://www.facebook.com/policies/
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;group-id&#125;/albums:
    get:
      summary: Get Group Albums
      description: The photo albums created for a Group.
      operationId: getGroupAlbums
      x-api-path-slug: 123groupid125albums-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Albums
  /me/albums:
    post:
      summary: Post Me Albums
      description: The photo albums created for a Group.
      operationId: postMeAlbums
      x-api-path-slug: mealbums-post
      parameters:
      - in: query
        name: message
        description: The description of the album, which will show up in news feed
          stories as the status message
        type: string
      - in: query
        name: name
        description: The name given to the album
        type: string
      - in: query
        name: Vector
        description: Vector
        type: string
      responses:
        200:
          description: OK
      tags:
      - Me
      - Albums
  /&#123;user-id&#125;/albums:
    get:
      summary: Get User Albums
      description: User Albums
      operationId: getUserAlbums
      x-api-path-slug: 123userid125albums-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      - in: query
        name: "200"
        description: Permissions error
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Albums
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