{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Water Act (CWA) Rest Services ECHO ICIS NPDES Inspection Types Lookup Service",
    "_postman_id": "6bf55914-bfb9-424d-a619-c8e8f329f67a",
    "description": "Returns the ICIS NPDES Compliance Monitoring Type Code and Description.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "6b925d00-304d-4d75-b48e-6df64b052646",
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
          "id": "942849a4-2f8f-4b00-8a10-fdedf07c9524"
        }
      ]
    },
    {
      "id": "e35f9633-1dc5-4d80-8471-c04de0fab277",
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
          "id": "357d8035-c2d6-419e-bbf6-86b8dc328872"
        }
      ]
    },
    {
      "id": "c24be270-2528-473c-9b07-39a4fb814469",
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
          "id": "23052e72-db8a-4114-a667-7b2bb82b1b17"
        }
      ]
    },
    {
      "id": "de8cfec1-5951-4292-92d4-a6cc2495c0e6",
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
          "id": "d2d86dac-bb01-4d3a-9da8-5f5bfac1716e"
        }
      ]
    },
    {
      "id": "05b3f3ae-aa9d-46f7-be8c-ba046c93f5a4",
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
          "id": "7b0d4ee8-1f5d-464e-ad77-562b7a1d33e1"
        }
      ]
    },
    {
      "id": "54a395ed-6500-4595-a4bc-f85478c620d4",
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
          "id": "9ee4f58d-5d51-4050-ad18-1c4c22b61806"
        }
      ]
    },
    {
      "id": "0a85d52a-9029-4c62-99a4-7d557d678268",
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
          "id": "346a2e6f-5e1b-4099-9abf-cc5c18b40079"
        }
      ]
    },
    {
      "id": "006ddc14-b4cd-4fa3-a21a-6201ccacfa7e",
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
          "id": "d1ef3452-480a-4a39-88d6-51d4c7f4fed1"
        }
      ]
    },
    {
      "id": "f88c540e-ce88-4bbe-a4d0-87ed8aa5ec56",
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
          "id": "71d4bd17-9395-4814-8a98-4c1b3cbb6cf3"
        }
      ]
    },
    {
      "id": "5d18825e-2993-457e-a3bb-fc1632ad690c",
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
          "id": "8eb87e1b-c95a-43c0-8499-9fc2b47d92cd"
        }
      ]
    },
    {
      "id": "7eb3a68d-6b18-4720-a285-3360ef7bdf4f",
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
          "id": "c67973ff-1bce-4dca-a7d7-f0eb4dea6704"
        }
      ]
    },
    {
      "id": "b85dc0de-6877-4ddc-b319-acaf7c0a5ecc",
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
          "id": "5f8408b9-dccb-43f9-850a-cdcd645f6a94"
        }
      ]
    },
    {
      "id": "17a434b6-3b7b-4cdf-933a-9e99d1b45d2d",
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
          "id": "75ad3de6-ee09-49b3-bd48-94ab1ed10866"
        }
      ]
    }
  ]
}