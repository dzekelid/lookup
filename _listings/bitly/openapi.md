swagger: "2.0"
x-collection-name: Bitly
x-complete: 1
info:
  title: Bitly User Metrics API
  description: the-bitly-user-metrics-api
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/link/lookup:
    get:
      summary: Get Link Lookup
      description: Get link lookup.
      operationId: getV3LinkLookup
      x-api-path-slug: v3linklookup-get
      parameters:
      - in: query
        name: url
        description: one or more long URLs to lookup
      responses:
        200:
          description: OK
      tags:
      - Link
      - Lookup
  /v3/user/link_lookup:
    get:
      summary: Get User Link Lookup
      description: Get user link lookup.
      operationId: getV3UserLinkLookup
      x-api-path-slug: v3userlink-lookup-get
      parameters:
      - in: query
        name: link
        description: one or more Bitlinks to lookup
      - in: query
        name: url
        description: one or more long URLs to lookup
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
      - Lookup