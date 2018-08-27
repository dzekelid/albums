swagger: "2.0"
x-collection-name: SugarSync
x-complete: 1
info:
  title: SugarSync  API
  description: the-sugarsync-service-presents-a-set-of-resources-that-your-application-can-access-through-the-platform-api--
  version: "1"
host: api.sugarsync.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /album/:
    get:
      summary: Retrieving Album Information
      description: To retrieve information about an album, an application submits
        an HTTP GET request to then          album resource that represents the album.
      operationId: retrieving-album-information
      x-api-path-slug: album-get
      parameters:
      - in: query
        name: max
        description: Positive integer
      - in: query
        name: order
        description: name, last_modified, size, or extension
      - in: query
        name: start
        description: 0 or positive integer
      responses:
        200:
          description: OK
      tags:
      - Album