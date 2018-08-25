---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Album Photos
  description: Lists photos for a given photo album
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/photo_album:
    post:
      summary: Photo Album2
      description: This method creates photo albums within a Meetup group
      operationId: photos
      x-api-path-slug: 2photo-album-post
      parameters:
      - in: query
        name: group_id
        description: Group to create the album in
        type: string
      - in: query
        name: title
        description: Title of the new album
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Albums
  /2/photos:
    ws:
      summary: WebSocket Photo Stream
      description: |-
        For browsers that support it, [WebSockets](http://dev.w3.org/html5/websockets/) is a more
        efficient alternative to the long-polling stream. This is a **push only** endpoint and will discard
        any messages received from the client after the socket is open.

        Because browser support for WebSockets is limited, we recommend that you consume this stream
        through the [must.js](https://github.com/meetup/must.js#readme) client, which can fallback to long-polling.
      operationId: streams
      x-api-path-slug: 2photos-ws
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Return recent photos with an mtime greater then the supplied
          time, in millisends since the epoch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Albums
  /2/photo_albums:
    get:
      summary: Photo Albums
      description: This method returns photo albums associated with Meetup groups.
        To create albums, see the corresponding write method.
      operationId: photos
      x-api-path-slug: 2photo-albums-get
      parameters:
      - in: query
        name: event_id
        description: Return photo albums for these event ids, separated by commas
        type: string
      - in: query
        name: group_id
        description: Return albums in groups with these ID, separated by commas
        type: string
      - in: query
        name: photo_album_id
        description: Return albums with these IDs, separated by commas
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
  /:urlname/photos:
    get:
      summary: Album Photos
      description: Lists of all photos uploaded for the group
      operationId: photos
      x-api-path-slug: urlnamephotos-get
      parameters:
      - in: query
        name: desc
        description: Controls directional order or listing
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: page
        description: Number of items to return per-page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photo_albums:
    get:
      summary: Photo Album List
      description: Gets a list a group photo albums in ascending order based on the
        time they were created
      operationId: photos
      x-api-path-slug: urlnamephoto-albums-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: offset
        description: Incrementing number used for pagination offsets
        type: string
      - in: query
        name: page
        description: Number of albums to return per page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photo_albums/:album_id:
    get:
      summary: Photo Album
      description: Gets information about a specific photo album
      operationId: photos
      x-api-path-slug: urlnamephoto-albumsalbum-id-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photo_albums/:album_id/photos:
    get:
      summary: Album Photos
      description: Lists photos for a given photo album
      operationId: photos
      x-api-path-slug: urlnamephoto-albumsalbum-idphotos-get
      parameters:
      - in: query
        name: desc
        description: Controls directional order or listing
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: page
        description: Number of items to return per-page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
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