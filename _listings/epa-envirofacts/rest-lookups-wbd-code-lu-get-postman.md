{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Water Act (CWA) Rest Services ECHO WBD Code Lookup Service",
    "_postman_id": "1333762f-c4e4-4879-86e1-822a684b2c91",
    "description": "USGS Watershed Boundary Dataset (WBD) Name lookup based on a supplied WBD Code and Watershed Level",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "d33b2d1d-f984-4c2d-8de6-3e1614dd5132",
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
          "id": "c224c603-d059-4131-928b-c87136a2a43e"
        }
      ]
    },
    {
      "id": "5b10ee85-5144-4043-affd-894b9822d8c5",
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
          "id": "d93fb723-05ac-449f-be54-48089b299d7a"
        }
      ]
    },
    {
      "id": "eb325ba9-f7dc-4bdb-a0b2-d27e14cbf20e",
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
          "id": "bc72fcbf-0b7d-4cb2-96bf-f0fca80ff7af"
        }
      ]
    },
    {
      "id": "a408440d-620a-4d19-98b0-87e7cb71bf08",
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
          "id": "3d15dc23-22c4-49dc-97d1-b01cd885220f"
        }
      ]
    },
    {
      "id": "de1ad967-1bc0-4d00-b276-301ef3489f76",
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
          "id": "e43b2dca-4189-4ba8-b926-7e3594048c70"
        }
      ]
    },
    {
      "id": "77ff2f9e-4cd4-4a23-a81d-bed3b50afd24",
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
          "id": "71a78d27-d19c-4fd5-9ca2-b4252b5dd429"
        }
      ]
    },
    {
      "id": "7b3cdef5-0ef8-4a21-bf5c-88106fe0a122",
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
          "id": "29901f02-1fdd-419a-b460-d5a1dd3591d4"
        }
      ]
    },
    {
      "id": "c732009f-7056-414c-bfe7-0dd395d163ff",
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
          "id": "7c3ae899-0142-4d04-b19c-1a6cdb06935a"
        }
      ]
    },
    {
      "id": "06771bb8-fad9-4e90-abc2-82c242d76fd2",
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
          "id": "b1745a03-ef17-4e95-87b7-b4cf388e3231"
        }
      ]
    },
    {
      "id": "3aa70bf8-b19b-4460-8983-6c7351f6a8f7",
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
          "id": "2b0e9b04-49ad-47e6-add6-07696ebc07f4"
        }
      ]
    },
    {
      "id": "6d47a5fa-6d34-4380-af17-4f0cb3ebe862",
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
          "id": "f72111a0-1e9c-4ea2-86ea-7e6ec76a696f"
        }
      ]
    },
    {
      "id": "b28c06be-41ab-42d7-bb9b-a44bd33458a4",
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
          "id": "2517cdae-55e9-4dd9-abaa-bd39271b4001"
        }
      ]
    },
    {
      "id": "4e5e7cb0-36f7-43e2-a86c-13b1b055f8c8",
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
          "id": "bc2f0e69-2647-4be4-8e85-b1fb1598fc14"
        }
      ]
    },
    {
      "id": "ac8e7ac8-3efc-4436-9fcb-1863ab12d113",
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
          "id": "0d15285b-8c06-49b0-b3d3-611b42b04b74"
        }
      ]
    },
    {
      "id": "cc834edb-912a-42d2-827f-cd9ceccb10a9",
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
          "id": "aececf3d-b321-458f-b9dd-cb48a063d7e3"
        }
      ]
    },
    {
      "id": "ac8d58a3-8e7a-4ca0-b2ba-3730e7c1e5f0",
      "name": "icis-limit-parameter-code-and-name-lookup-based-on-the-supply-of-a-partial-parameter-name--npdes--na",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.npdes_parameters?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "ICIS Limit Parameter Code and Name lookup based on the supply of a partial parameter name. (NPDES = National Pollutant Discharge Elimination System)"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "ed7e839d-6620-4c8b-92ab-70a800342ff2"
        }
      ]
    },
    {
      "id": "3a66fde5-3e67-4f15-97d9-39eed0acf0d6",
      "name": "usgs-watershed-boundary-dataset-wbd-name-lookup-based-on-a-supplied-wbd-code-and-watershed-level",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.wbd_code_lu?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "USGS Watershed Boundary Dataset (WBD) Name lookup based on a supplied WBD Code and Watershed Level"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "25b88db5-1e6f-4a24-aa04-d5e4bd4afcca"
        }
      ]
    }
  ]
}