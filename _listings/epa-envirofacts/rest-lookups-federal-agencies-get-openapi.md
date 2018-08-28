---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Water Act
    (CWA) Rest Services ECHO Federal Agency Lookup Service
  description: Look up Federal Agency Code
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest_lookups.wbd_name_lu:
    get:
      summary: ECHO WBD Name Lookup Service
      description: USGS Watershed Boundary Dataset (WBD) Code lookup based on a supplied
        WBD Name and Watershed Level
      operationId: usgs-watershed-boundary-dataset-wbd-code-lookup-based-on-a-supplied-wbd-name-and-watershed-level
      x-api-path-slug: rest-lookups-wbd-name-lu-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - WBD
      - Name
      - Lookup
      - Service
  /rest_lookups.wbd_code_lu:
    get:
      summary: ECHO WBD Code Lookup Service
      description: USGS Watershed Boundary Dataset (WBD) Name lookup based on a supplied
        WBD Code and Watershed Level
      operationId: usgs-watershed-boundary-dataset-wbd-name-lookup-based-on-a-supplied-wbd-code-and-watershed-level
      x-api-path-slug: rest-lookups-wbd-code-lu-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - WBD
      - Code
      - Lookup
      - Service
  /rest_lookups.npdes_parameters:
    get:
      summary: ECHO NPDES Parameters Lookup Service
      description: ICIS Limit Parameter Code and Name lookup based on the supply of
        a partial parameter name. (NPDES = National Pollutant Discharge Elimination
        System)
      operationId: icis-limit-parameter-code-and-name-lookup-based-on-the-supply-of-a-partial-parameter-name--npdes--na
      x-api-path-slug: rest-lookups-npdes-parameters-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - NPDES
      - Parameters
      - Lookup
      - Service
  /rest_lookups.naics_codes:
    get:
      summary: ECHO NAICS Codes Lookup Service
      description: ""
      operationId: ""
      x-api-path-slug: rest-lookups-naics-codes-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - NAICS
      - Codes
      - Lookup
      - Service
  /rest_lookups.icis_law_sections:
    get:
      summary: ECHO ICIS Law Sections Lookup Service
      description: Returns the ICIS Law Section Descriptions.
      operationId: returns-the-icis-law-section-descriptions-
      x-api-path-slug: rest-lookups-icis-law-sections-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - ICIS
      - Law
      - Sections
      - Lookup
      - Service
  /rest_lookups.icis_inspection_types:
    get:
      summary: ECHO ICIS NPDES Inspection Types Lookup Service
      description: Returns the ICIS NPDES Compliance Monitoring Type Code and Description.
      operationId: returns-the-icis-npdes-compliance-monitoring-type-code-and-description-
      x-api-path-slug: rest-lookups-icis-inspection-types-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - ICIS
      - NPDES
      - Inspection
      - Types
      - Lookup
      - Service
  /rest_lookups.federal_agencies:
    get:
      summary: ECHO Federal Agency Lookup Service
      description: Look up Federal Agency Code
      operationId: look-up-federal-agency-code
      x-api-path-slug: rest-lookups-federal-agencies-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - Federal
      - Agency
      - Lookup
      - Service
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