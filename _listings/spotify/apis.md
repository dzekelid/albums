---
name: Spotify
x-slug: spotify
description: Spotify is a digital music service that gives you access to millions
  of songs.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
x-kinRank: "8"
x-alexaRank: "133"
tags: Albums
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/apis.md
specificationVersion: "0.14"
apis:
- name: Spotify Get Albums
  x-api-slug: spotify
  description: '[Get Several Albums](https://developer.spotify.com/web-api/get-several-albums/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//albums
  tags: Music,Albums
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/albums-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/albums-get-openapi.md
- name: Spotify Get Album
  x-api-slug: spotify
  description: '[Get an Album](https://developer.spotify.com/web-api/get-album/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//albums/{id}
  tags: Music,Albums
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/albumsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/albumsid-get-openapi.md
- name: Spotify Get Artist Albums
  x-api-slug: spotify
  description: '[Get an Artist''s Albums](https://developer.spotify.com/web-api/get-artists-albums/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//artists/{id}/albums
  tags: Music,Artists,Albums
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/artistsidalbums-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/artistsidalbums-get-openapi.md
- name: Spotify
  x-api-slug: spotify
  description: Spotify is a digital music service that gives you access to millions
    of songs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1
  tags: Albums
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/albums/master/_listings/spotify/openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://developer.spotify.com/wp-content/uploads/apis.json
- type: x-android-sdk
  url: https://developer.spotify.com/technologies/spotify-android-sdk/
- type: x-application-gallery
  url: https://developer.spotify.com/my-applications/
- type: x-application-gallery
  url: https://developer.spotify.com/showcase/
- type: x-base-url
  url: https://api.spotify.com
- type: x-blog
  url: http://www.spotify.com/blog/
- type: x-blog-rss
  url: http://www.spotify.com/blog/feed
- type: x-change-log
  url: https://developer.spotify.com/web-api/change-log/
- type: x-console
  url: https://developer.spotify.com/web-api/console/
- type: x-crunchbase
  url: https://crunchbase.com/organization/spotify
- type: x-crunchbase
  url: http://www.crunchbase.com/company/spotify
- type: x-developer
  url: https://developer.spotify.com/
- type: x-email
  url: office@spotify.com
- type: x-ios-sdk
  url: https://developer.spotify.com/technologies/spotify-ios-sdk/
- type: x-issues
  url: https://github.com/spotify/web-api/issues
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/spotify
- type: x-terms-of-service
  url: https://developer.spotify.com/developer-terms-of-use/
- type: x-twitter
  url: https://twitter.com/SpotifyPlatform
- type: x-twitter
  url: https://twitter.com/spotify
- type: x-github
  url: https://github.com/spotify
- type: x-website
  url: http://www.spotify.com
- type: x-website
  url: http://spotify.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---