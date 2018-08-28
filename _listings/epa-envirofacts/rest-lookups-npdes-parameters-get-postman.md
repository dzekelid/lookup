{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Water Act (CWA) Rest Services ECHO NPDES Parameters Lookup Service",
    "_postman_id": "a67c9a7d-48b8-4d50-acf4-0162f2c6b011",
    "description": "ICIS Limit Parameter Code and Name lookup based on the supply of a partial parameter name. (NPDES = National Pollutant Discharge Elimination System)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "c8fc41c8-d9a6-42ae-a658-708857998013",
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
          "id": "6565b510-7cef-48ea-97dd-d69b78beb4d6"
        }
      ]
    },
    {
      "id": "3cb79a6c-fe2d-4ea8-bd95-61b75c3b261d",
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
          "id": "7aa8115f-0c29-4f1c-bd7b-cb87e9424442"
        }
      ]
    },
    {
      "id": "0175ab4f-daa4-4808-9a0c-c568ec4e978f",
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
          "id": "4236b889-5d26-4644-be3b-e73ec8cf4658"
        }
      ]
    },
    {
      "id": "80507d8e-2e07-4376-90b3-99d02be60ab3",
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
          "id": "cdf93939-4564-497d-b558-eee78b5ac926"
        }
      ]
    },
    {
      "id": "a768554d-1f56-4f1e-a7b4-c1530d83ceeb",
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
          "id": "3c803417-c2a5-4649-a4b4-e380c95d5807"
        }
      ]
    },
    {
      "id": "fb8f58dd-1ba3-4c39-b971-99ad1d350709",
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
          "id": "a0a67876-9c4a-4565-9ff7-93452cc89f4f"
        }
      ]
    },
    {
      "id": "800b010f-d413-40b5-9839-bd178450b20d",
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
          "id": "33055710-c0dd-4556-b8d7-4df62394005d"
        }
      ]
    },
    {
      "id": "17e5a6a5-3061-4809-88a5-adf91d207d21",
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
          "id": "325544a5-55d3-45c3-a02c-95fb0c080ddb"
        }
      ]
    },
    {
      "id": "92f33c82-3bc7-4898-b22b-70a12f85b765",
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
          "id": "bc1fee0c-7f85-447e-9653-ea96d40d3a6a"
        }
      ]
    },
    {
      "id": "7bef5c70-4af3-4b4c-a1dc-60a6f59c2e7e",
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
          "id": "2db79e8d-d4d8-418d-a77d-f60d1b089fb1"
        }
      ]
    },
    {
      "id": "9782fb83-7c6d-4d8d-b858-2b67bd391a61",
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
          "id": "172c62e8-b8b0-40eb-b74c-90188bcd70e7"
        }
      ]
    },
    {
      "id": "785bb804-e00e-4710-b974-9e3fe60652b6",
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
          "id": "8de81ab2-b63a-484d-8dc6-35e71707db43"
        }
      ]
    },
    {
      "id": "9976064e-4287-4912-99cd-db58a2a0d2ed",
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
          "id": "c080ef37-55fb-4854-935b-89895cfdd120"
        }
      ]
    },
    {
      "id": "02345f45-bff6-4c2c-9ee3-441523c60497",
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
          "id": "c590d84a-9ed9-49bc-a8d4-969b2984cd09"
        }
      ]
    },
    {
      "id": "6f0a7de0-f4ad-4a3b-bd00-4a6e589e2112",
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
          "id": "34e29e94-5f9c-47ca-b2aa-aea86ea4ea26"
        }
      ]
    },
    {
      "id": "27097057-3be3-4ab5-abad-6cbc24ea4c76",
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
          "id": "5fb135fe-1fef-460f-8485-812271e2d1ae"
        }
      ]
    }
  ]
}