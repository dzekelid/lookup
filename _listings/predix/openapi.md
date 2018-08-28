swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/tenant/profile:
    get:
      summary: Lookup Tenant by Subdomain
      description: Lookup tenant by subdomain.
      operationId: getTenantBySubdomainUsingGET
      x-api-path-slug: v1tenantprofile-get
      parameters:
      - in: header
        name: TMS-Zone-Subdomain
      responses:
        200:
          description: Successful response
      tags:
      - Lookup
      - Tenant
      - By
      - Subdomain
  /v1/tenant/profile/service/{serviceName}:
    get:
      summary: Lookup Tenant service by Subdomain
      description: Lookup tenant service by subdomain.
      operationId: getTenantServiceBySubdomainUsingGET
      x-api-path-slug: v1tenantprofileserviceservicename-get
      parameters:
      - in: path
        name: serviceName
        description: serviceName
      - in: header
        name: TMS-Zone-Subdomain
      responses:
        200:
          description: Successful response
      tags:
      - Lookup
      - Tenant
      - Service
      - By
      - Subdomain
  /v2/tenants/{tenantSubdomain}:
    get:
      summary: Lookup Tenant by Subdomain
      description: Lookup tenant by subdomain.
      operationId: getTenantProfileBySubdomainUsingGET
      x-api-path-slug: v2tenantstenantsubdomain-get
      parameters:
      - in: path
        name: tenantSubdomain
        description: tenantSubdomain
      responses:
        200:
          description: Successful response
      tags:
      - Lookup
      - Tenant
      - By
      - Subdomain
  /v2/tenants/{tenantSubdomain}/service-instances/{serviceInstanceName}:
    get:
      summary: Lookup Tenant Service by Subdomain
      description: Lookup tenant service by subdomain.
      operationId: getTenantServiceBySubdomainUsingGET_1
      x-api-path-slug: v2tenantstenantsubdomainserviceinstancesserviceinstancename-get
      parameters:
      - in: path
        name: serviceInstanceName
        description: serviceInstanceName
      - in: path
        name: tenantSubdomain
        description: tenantSubdomain
      responses:
        200:
          description: Successful response
      tags:
      - Lookup
      - Tenant
      - Service
      - By
      - Subdomain
  /v2/tenants/{tenantSubdomain}/status:
    get:
      summary: Lookup Tenant status by Subdomain
      description: Lookup tenant status by subdomain.
      operationId: getTenantProfileStatusBySubdomainUsingGET
      x-api-path-slug: v2tenantstenantsubdomainstatus-get
      parameters:
      - in: path
        name: tenantSubdomain
        description: tenantSubdomain
      responses:
        200:
          description: Successful response
      tags:
      - Lookup
      - Tenant
      - Status
      - By
      - Subdomain