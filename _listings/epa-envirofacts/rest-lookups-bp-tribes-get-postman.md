{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Water Act (CWA) Rest Services ECHO BP Tribes Lookup Service",
    "_postman_id": "2cd839f4-8525-48d6-b3fa-c798bab82523",
    "description": "Returns the EPA Standard Indian Tribes and Native Alaskan Villages tribal_id and tribe_name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "44224186-2029-4369-b50f-43c1eeb1415f",
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
          "id": "48db7c46-674f-4b46-80c9-6760eefee726"
        }
      ]
    },
    {
      "id": "9065a964-b37d-4bcc-88bb-940f40060444",
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
          "id": "c506eed2-f3f3-4bf6-b39e-4b1b0821e033"
        }
      ]
    },
    {
      "id": "1b26acb9-01e7-4626-b330-8b93f52d6066",
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
          "id": "12a196ff-6863-41d3-af16-aafde93b40bf"
        }
      ]
    },
    {
      "id": "22da85ab-79a4-4bbf-bd50-8f649ba630e1",
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
          "id": "03af0997-e5ea-40ab-b03e-6fc1b773f333"
        }
      ]
    },
    {
      "id": "bd06b026-0f65-4d76-b03a-702176cde01d",
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
          "id": "d7619651-5b20-475c-86b0-b3d261967c94"
        }
      ]
    },
    {
      "id": "1e3a294f-cbc5-400e-b53d-9fd3f5dad54a",
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
          "id": "df76abb0-5471-4cf4-81da-73c8e4933bdd"
        }
      ]
    },
    {
      "id": "d8676fa1-4d2e-4f36-898e-98816ca45cb0",
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
          "id": "a774c498-bdf3-4e32-aae6-a410f21e3d99"
        }
      ]
    },
    {
      "id": "ca2fbb15-c794-4795-b949-7112e4b5ec66",
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
          "id": "3ae7ffce-d6a2-428f-8454-80042844aff6"
        }
      ]
    },
    {
      "id": "3b622fc1-9d41-4089-b1cd-f71cc71685e4",
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
          "id": "ce07e7f8-584c-4fe4-8a3b-ba6ed2dd8642"
        }
      ]
    }
  ]
}