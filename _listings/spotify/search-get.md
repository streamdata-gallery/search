---
swagger: "2.0"
info:
  title: Spotify Search
  description: '[Search for an Item](https://developer.spotify.com/web-api/search-item/)'
  version: v1
host: api.spotify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Search
      description: '[Search for an Item](https://developer'
      operationId: search-for-an-itemhttpsdeveloperspotifycomwebapisearchitem
      parameters:
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: offset
        description: The index of the first item to return
      - in: query
        name: q
        description: The search query's keywords (and optional field filters)
      - in: query
        name: type
        description: A comma-separated list of item types to search across
      responses:
        200:
          description: OK
      tags:
      - music
      - search
definitions:
  album:
    properties:
      album_type:
        description: This is a default description.
        type: put
      artists:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      copyrights:
        description: This is a default description.
        type: put
      external_ids:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      genres:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
  album-simple:
    properties:
      album_type:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  album-simple-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  album-track-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  artist:
    properties:
      external_urls:
        description: This is a default description.
        type: put
      genres:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      popularity:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  artist-simple:
    properties:
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  category:
    properties:
      href:
        description: This is a default description.
        type: put
      icons:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  category-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  current-user-profile:
    properties:
      birthdate:
        description: This is a default description.
        type: put
      country:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      email:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      product:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  featured-playlists:
    properties:
      message:
        description: This is a default description.
        type: put
  followers:
    properties:
      href:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  image:
    properties:
      height:
        description: This is a default description.
        type: put
      url:
        description: This is a default description.
        type: put
      width:
        description: This is a default description.
        type: put
  playlist:
    properties:
      collaborative:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      followers:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      public:
        description: This is a default description.
        type: put
      snapshot_id:
        description: This is a default description.
        type: put
  playlist-simple:
    properties:
      collaborative:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      public:
        description: This is a default description.
        type: put
      snapshot_id:
        description: This is a default description.
        type: put
      tracks:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  playlist-simple-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  playlist-snapshot:
    properties:
      snapshot_id:
        description: This is a default description.
        type: put
  playlist-track:
    properties:
      added_at:
        description: This is a default description.
        type: put
      is_local:
        description: This is a default description.
        type: put
  playlist-track-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  saved-track:
    properties:
      added_at:
        description: This is a default description.
        type: put
  saved-track-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  search:
    properties:
      albums:
        description: This is a default description.
        type: put
      artists:
        description: This is a default description.
        type: put
      tracks:
        description: This is a default description.
        type: put
  track:
    properties:
      artists:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      disc_number:
        description: This is a default description.
        type: put
      duration_ms:
        description: This is a default description.
        type: put
      explicit:
        description: This is a default description.
        type: put
      external_ids:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      is_playable:
        description: This is a default description.
        type: put
  track-simple:
    properties:
      artists:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      disc_number:
        description: This is a default description.
        type: put
      duration_ms:
        description: This is a default description.
        type: put
      explicit:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      is_playable:
        description: This is a default description.
        type: put
      linked_from:
        description: This is a default description.
        type: put
  track-simple-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  user-followed:
    properties:
      artists:
        description: This is a default description.
        type: put
  user-profile:
    properties:
      displayName:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
x-collection-name: Spotify
x-streamrank:
  polling_total_time_average: "0.1"
  polling_size_download_average: "4080.73"
  streaming_total_time_average: "0.06"
  streaming_size_download_average: "2046.76"
  change_yes: "4"
  change_no: "195"
  time_percentage: "45"
  size_percentage: "50"
  change_percentage: "2"
  last_run: "2018-05-06"
  days_run: "1"
  minute_run: "0"
---