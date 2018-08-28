{
  "info": {
    "name": "OpenStreetMap OSM - Address lookup",
    "_postman_id": "c528d61b-6bf4-45a0-aaa6-d656f6a03a3c",
    "description": "[Full description of the service:](http://wiki.openstreetmap.org/wiki/Nominatim#Address_lookup)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Maps",
      "item": [
        {
          "id": "b11cdd13-ec9a-44aa-99c5-13023e72876a",
          "name": "LookupGet",
          "request": {
            "url": "http:// http://nominatim.openstreetmap.org/lookup?format=%7B%7D&osm_ids=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "[Full description of the service:](http://wiki.openstreetmap.org/wiki/Nominatim#Address_lookup)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4db7325d-3c50-4c39-88d6-5e0bb3f48157"
            }
          ]
        }
      ]
    }
  ]
}