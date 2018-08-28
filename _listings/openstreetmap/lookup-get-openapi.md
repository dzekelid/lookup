---
swagger: "2.0"
x-collection-name: OpenStreetMap
x-complete: 0
info:
  title: OpenStreetMap OSM - Address lookup
  description: '[Full description of the service:](http://wiki.openstreetmap.org/wiki/Nominatim#Address_lookup)'
  version: 1.0.0
host: ' http:'
basePath: //nominatim.openstreetmap.org
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lookup:
    get:
      summary: OSM - Address lookup
      description: '[Full description of the service:](http://wiki.openstreetmap.org/wiki/Nominatim#Address_lookup)'
      operationId: LookupGet
      x-api-path-slug: lookup-get
      parameters:
      - in: query
        name: format
      - in: query
        name: osm_ids
      responses:
        200:
          description: OK
      tags:
      - Maps
      - OSM
      - Address
      - Lookup
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