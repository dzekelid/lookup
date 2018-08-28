---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 0
info:
  title: Infermedica Get Lookup
  description: Returns a single observation matching given phrase.
  version: v2
host: api.infermedica.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lookup:
    get:
      summary: Get Lookup
      description: Returns a single observation matching given phrase.
      operationId: getLookup
      x-api-path-slug: lookup-get
      parameters:
      - in: query
        name: phrase
        description: phrase to match
      - in: query
        name: sex
        description: sex filter
      responses:
        200:
          description: OK
      tags:
      - Healthcare
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