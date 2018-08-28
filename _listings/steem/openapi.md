swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lookup_witness_accounts:
    get:
      summary: lookup_witness_accounts
      description: lookup_witness_accounts regex search
      operationId: lookup-witness-accounts-regex-search
      x-api-path-slug: lookup-witness-accounts-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: lowerBoundName
        description: lowerBoundName
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Witness
      - Accounts
  /lookup_account_names:
    get:
      summary: lookup_account_names
      description: lookup_account_names example of accountNames ["good-karma", "fabien"]
      operationId: lookup-account-names-example-of-accountnames-goodkarma-fabien
      x-api-path-slug: lookup-account-names-get
      parameters:
      - in: query
        name: accountNames
        description: accountNames [good-karma, fabien]
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Account
      - Names
  /lookup_accounts:
    get:
      summary: lookup_accounts
      description: lookup_accounts regex search
      operationId: lookup-accounts-regex-search
      x-api-path-slug: lookup-accounts-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: lowerBoundName
        description: lowerBoundName
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Accounts