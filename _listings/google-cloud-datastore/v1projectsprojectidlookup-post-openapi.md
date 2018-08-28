---
swagger: "2.0"
x-collection-name: Google Cloud Datastore
x-complete: 0
info:
  title: Google Cloud Datastore API Lookup Entity by Key
  description: Looks up entities by key.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: datastore.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}:lookup:
    post:
      summary: Lookup Entity by Key
      description: Looks up entities by key.
      operationId: datastore.projects.lookup
      x-api-path-slug: v1projectsprojectidlookup-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
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