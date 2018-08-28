swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 1
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Safe Drinking
    Water Act
  description: enforcement-and-compliance-history-online-echo-is-a-tool-developed-and-maintained-by-epas-office-of-enforcement-and-compliance-assurance-for-public-use--echo-provides-integrated-compliance-and-enforcement-information-for-about-800000-regulated-facilities-nationwide-brbrsdw-rest-services-provides-multiple-service-endpoints-each-with-specific-capabilities-to-search-and-retrieve-data-on-public-water-systems-regulated-under-the-safe-drinking-water-act-sdwa--the-returned-results-reflect-data-drawn-from-epas-federal-safe-drinking-water-information-system-sdwis-database-brbrthe-get-systems-get-qid-and-get-download-end-points-are-meant-to-be-used-together-brbrthe-recommended-use-scenario-for-get-systems-get-qid-and-get-downoad-isbrbrb1bnbsp-use-get-systems-to-validate-passed-query-parameters-obtain-summary-statistics-and-to-obtain-a-query-id-qid---qids-are-time-sensitive-and-will-be-valid-for-approximately-30-minutes-brb2bnbsp-use-get-qid-with-the-returned-qid-to-paginate-through-arrays-of-water-system-results-brb3bnbsp-use-get-download-with-the-returned-qid-to-generate-a-comma-separated-value-csv-file-of-water-system-information-that-meets-the-qid-query-criteria-brbruse-the-qcolumns-parameter-to-customize-your-search-results---use-the-metdata-service-endpoint-for-a-list-of-available-output-objects-their-column-ids-and-their-definitions-to-help-you-build-your-customized-output--brbradditional-echo-resourcesnbspnbsp-a-hrefhttpsecho-epa-govtoolswebservicesweb-servicesa-a-hrefhttpsecho-epa-govresourcesechodataaboutthedataabout-echos-dataa-a-hrefhttpsecho-epa-govtoolsdatadownloadsdata-downloadsabr
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
  /rest_lookups.cwa_pollutants:
    get:
      summary: ECHO CWA Pollutants Lookup Service
      description: ""
      operationId: ""
      x-api-path-slug: rest-lookups-cwa-pollutants-get
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
      - CWA
      - Pollutants
      - Lookup
      - Service
  /rest_lookups.cwa_parameters:
    get:
      summary: ECHO CWA Parameter Lookup Service
      description: Look up Clean Water Act parameter codes and descriptions in the
        Integrated Compliance Information System - National Pollutant Discharge Elimination
        System (ICIS-NPDES) by code or term.
      operationId: look-up-clean-water-act-parameter-codes-and-descriptions-in-the-integrated-compliance-information-sy
      x-api-path-slug: rest-lookups-cwa-parameters-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - CWA
      - Parameter
      - Lookup
      - Service
  /rest_lookups.bp_tribes:
    get:
      summary: ECHO BP Tribes Lookup Service
      description: Returns the EPA Standard Indian Tribes and Native Alaskan Villages
        tribal_id and tribe_name.
      operationId: returns-the-epa-standard-indian-tribes-and-native-alaskan-villages-tribal-id-and-tribe-name-
      x-api-path-slug: rest-lookups-bp-tribes-get
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
      - BP
      - Tribes
      - Lookup
      - Service