---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 1
info:
  title: Infermedica
  description: empower-your-healthcare-services-with-intelligent-diagnostic-insights-of-infermedica-api-
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
---