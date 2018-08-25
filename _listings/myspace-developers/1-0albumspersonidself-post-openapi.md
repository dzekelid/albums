---
swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 0
info:
  title: My Space Post Albums Personid Self
  description: Adding an Album.
  version: 1.0.0
host: api.myspace.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1.0/albums/{personId}/@self/{albumId}:
    put:
      summary: Put Albums Personid Self Albums
      description: Update an Album.
      operationId: 1.0.albums.personId._self.albumId.put
      x-api-path-slug: 1-0albumspersonidselfalbumid-put
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album should be returned
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
      - AlbumId
    get:
      summary: Get Albums Personid Self Albums
      description: Retrieves an album.
      operationId: 1.0.albums.personId._self.albumId.get
      x-api-path-slug: 1-0albumspersonidselfalbumid-get
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album should be returned
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
      - AlbumId
  /1.0/albums/{personId}/@self:
    post:
      summary: Post Albums Personid Self
      description: Adding an Album.
      operationId: 1.0.albums.personId._self.post
      x-api-path-slug: 1-0albumspersonidself-post
      parameters:
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
    get:
      summary: Get Albums Personid Self
      description: Retrieves the current user's albums.
      operationId: 1.0.albums.personId._self.get
      x-api-path-slug: 1-0albumspersonidself-get
      parameters:
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - Albums
      - People
      - Self
  /1.0/albums/@supportedFields:
    get:
      summary: Get Albums Supported Fields
      description: Retrieves all supported fields.
      operationId: 1.0.albums._supportedFields.get
      x-api-path-slug: 1-0albumssupportedfields-get
      parameters:
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - Albums
      - Supported
      - Fields
  /1.0/mediaitemcomments/{personId}/@self/{albumId}/{mediaItemId}:
    get:
      summary: Get Mediaitemcomments Personid Self Albums Mediaitemid
      description: Retrieves item comments from a specified album.
      operationId: 1.0.mediaitemcomments.personId._self.albumId.mediaItemId.get
      x-api-path-slug: 1-0mediaitemcommentspersonidselfalbumidmediaitemid-get
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album from the group identified by {selector}
          should be returned
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: mediaItemId
        description: Indicates which single media item from the album identified by
          {albumId} should be returned
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - Mediaitemcomments
      - People
      - Self
      - AlbumId
      - MediaItemId
  /1.0/mediaItems/{personId}/@self/{albumId}:
    post:
      summary: Post Mediaitems Personid Self Albums
      description: Adds items from a specified album.
      operationId: 1.0.mediaItems.personId._self.albumId.post
      x-api-path-slug: 1-0mediaitemspersonidselfalbumid-post
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album from the group identified by {selector}
          should be returned
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - AlbumId
    get:
      summary: Get Mediaitems Personid Self Albums
      description: Retrieves items from a specified album.
      operationId: 1.0.mediaItems.personId._self.albumId.get
      x-api-path-slug: 1-0mediaitemspersonidselfalbumid-get
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album from the group identified by {selector}
          should be returned
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - AlbumId
  /1.0/mediaItems/{personId}/@self/{albumId}/{mediaItemId}:
    put:
      summary: Put Mediaitems Personid Self Albums Mediaitemid
      description: Updates an item from a specified album.
      operationId: 1.0.mediaItems.personId._self.albumId.mediaItemId.put
      x-api-path-slug: 1-0mediaitemspersonidselfalbumidmediaitemid-put
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album from the group identified by {selector}
          should be returned
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: header
        name: Content-Type
        description: Specifies Content Type
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: mediaItemId
        description: Indicates which single media item from the album identified by
          {albumId} should be returned
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - AlbumId
      - MediaItemId
    get:
      summary: Get Mediaitems Personid Self Albums Mediaitemid
      description: Retrieves an item from a specified album.
      operationId: 1.0.mediaItems.personId._self.albumId.mediaItemId.get
      x-api-path-slug: 1-0mediaitemspersonidselfalbumidmediaitemid-get
      parameters:
      - in: path
        name: albumId
        description: Indicates which single album from the group identified by {selector}
          should be returned
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: path
        name: mediaItemId
        description: Indicates which single media item from the album identified by
          {albumId} should be returned
      - in: query
        name: msPrivacyLevel
        description: MySpace specific field
      - in: path
        name: personId
        description: The persons identifier
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      responses:
        200:
          description: OK
      tags:
      - MediaItems
      - People
      - Self
      - AlbumId
      - MediaItemId
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