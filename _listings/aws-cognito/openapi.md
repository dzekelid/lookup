---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=LookupDeveloperIdentity:
    get:
      summary: Lookup Developer Identity
      description: |-
        Retrieves the IdentityID associated with a
                    DeveloperUserIdentifier or the list of
                 DeveloperUserIdentifiers associated with an IdentityId for an
                 existing identity.
      operationId: lookupDeveloperIdentity
      x-api-path-slug: actionlookupdeveloperidentity-get
      parameters:
      - in: query
        name: DeveloperUserIdentifier
        description: A unique ID used by your backend authentication process to identify
          a user
        type: string
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of identities to return
        type: string
      - in: query
        name: NextToken
        description: A pagination token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Developer Identities
---