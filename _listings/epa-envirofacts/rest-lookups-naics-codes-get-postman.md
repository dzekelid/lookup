{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Water Act (CWA) Rest Services ECHO NAICS Codes Lookup Service",
    "_postman_id": "45655cd9-6a3f-4230-a584-00614135cc8c",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "29481c20-c693-4cbe-a24d-9b71ba38e132",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-geojson-of-the-fac",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_download?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return GeoJSON of the facilities found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "940c19c7-0f3a-43b4-9771-a4856b8cd233"
        }
      ]
    },
    {
      "id": "4a2a234d-cd48-464b-92ef-1efb131babd2",
      "name": "validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_facilities?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Validates query search parameters and returns query identifier.  Use the responseset parameter to set the page size"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "4d4f4fa9-ed05-438c-8eca-db11b0528c0d"
        }
      ]
    },
    {
      "id": "f33f115a-a293-4062-90b7-5c81723531ab",
      "name": "returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_facility_info?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns either an array of Facilities or an array of Clusters that meet the specified search criteria."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "890e1bec-ee13-4170-b1ef-a85677182abe"
        }
      ]
    },
    {
      "id": "419e8cc7-5d80-4d50-a91b-30cc156bc6e4",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_geojson?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return a comma sepated vaule (CSV) file of the facilities found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c1d281c8-7163-417e-aec5-222c14b66173"
        }
      ]
    },
    {
      "id": "add4c7f0-a04b-452f-879a-444adf8790dd",
      "name": "based-on-the-qid-obtained-from-a-clustered-get-facility-info-query-download-cluster-facility-informa",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_info_clusters?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a clustered get_facility_info query, download cluster facility information as either a CSV or GEOJSON file."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "f4a9bd43-c945-4d69-bd02-56a7581151d4"
        }
      ]
    },
    {
      "id": "cb48fe44-149c-422f-9669-1e534d5ba68d",
      "name": "the-purpose-of-the-get-map-service-is-to-display-facility-coordinates-and-facility-clusters-related-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_map?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The purpose of the GET_MAP service is to display facility coordinates and facility clusters related to a get_facilities facility query. Currently, the maximum number of coordinates returned is 500. GET_MAP performs automatic clustering at the state, county, and zip code levels to maximize the number of coordinates returned."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cf13de09-975b-44fd-8ac4-0957c1360363"
        }
      ]
    },
    {
      "id": "7bbfb364-a666-4538-9893-3e69b87ce5ea",
      "name": "get-qid-is-passed-with-a-query-id-corresponding-to-a-previously-run-get-facilities-query--it-then-re",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_qid?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "GET_QID is passed with a query ID corresponding to a previously run get_facilities query. It then returns a Facility object containing all matching facilities. The main purpose of GET_QID is for large querysets that contain multiple pages (responsesets) of output. GET_QID allows for pagination and for the selection and sorting of columns."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "08d6845c-46da-4b40-a78a-78b4e54dad1d"
        }
      ]
    },
    {
      "id": "c62790d0-71ff-4651-8b7b-8aa335e2b49d",
      "name": "returns-the-json-object-name-and-columnid-for-usage-with-the-qcolumns-parameter-for-get-qid-get-faci",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.metadata?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the JSON Object Name and ColumnId for usage with the qcolumns parameter for get_qid, get_facility_info and other service endpoints."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "67f4b8d9-0357-4d25-865f-689dd60457cc"
        }
      ]
    },
    {
      "id": "29cff6b9-92bd-4168-8324-6ba265b0c28a",
      "name": "returns-the-epa-standard-indian-tribes-and-native-alaskan-villages-tribal-id-and-tribe-name-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.bp_tribes?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the EPA Standard Indian Tribes and Native Alaskan Villages tribal_id and tribe_name."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "88de6d46-a979-4456-8bc2-730706aa07af"
        }
      ]
    },
    {
      "id": "cd4b7f18-d65c-4b47-acdc-f1edba64a7b6",
      "name": "look-up-clean-water-act-parameter-codes-and-descriptions-in-the-integrated-compliance-information-sy",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.cwa_parameters?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Look up Clean Water Act parameter codes and descriptions in the Integrated Compliance Information System - National Pollutant Discharge Elimination System (ICIS-NPDES) by code or term."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "336840f1-4835-4e78-9d83-be3d38f3d4f1"
        }
      ]
    },
    {
      "id": "437c12af-2eb5-4b0b-94f0-bb6e5250cc84",
      "name": "ECHO CWA Pollutants Lookup Service",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.cwa_pollutants?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "ECHO CWA Pollutants Lookup Service"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "a2090e1f-1171-473b-9201-bbcc62790e87"
        }
      ]
    },
    {
      "id": "c7969f88-6e93-45c4-ab64-478e4bffafd6",
      "name": "look-up-federal-agency-code",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.federal_agencies?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Look up Federal Agency Code"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fa145fa0-2d2d-4464-9225-2a1b527d379d"
        }
      ]
    },
    {
      "id": "9ee3f81a-3c91-4351-a71f-f10c1fd696c1",
      "name": "returns-the-icis-npdes-compliance-monitoring-type-code-and-description-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.icis_inspection_types?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the ICIS NPDES Compliance Monitoring Type Code and Description."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7ef002cf-eaba-4f9c-94c8-1ff5640be53d"
        }
      ]
    },
    {
      "id": "91cb3569-6a26-4ff9-a115-ef1040287e7c",
      "name": "returns-the-icis-law-section-descriptions-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.icis_law_sections?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the ICIS Law Section Descriptions."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3d2bb7b0-c76b-4695-b189-095e5e1bac6a"
        }
      ]
    },
    {
      "id": "a84bbfec-8b82-450b-b9e0-e93dceef41d5",
      "name": "ECHO NAICS Codes Lookup Service",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.naics_codes?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "ECHO NAICS Codes Lookup Service"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "164d6743-3ab4-4c2f-9f47-a0bd4f919562"
        }
      ]
    }
  ]
}