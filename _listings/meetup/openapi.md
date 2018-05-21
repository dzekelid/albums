---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  description: the-meetup-api-provides-simple-restful-http-and-streaming-interfaces-for-exploring-and-interacting-meetup-platform-from-your-own-apps-the-api-is-a-set-of-core-methods-and-a-common-request-format-these-are-combined-to-form-a-url-that-returns-the-information-you-want-
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
        description: ' Title of the new album'
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
---