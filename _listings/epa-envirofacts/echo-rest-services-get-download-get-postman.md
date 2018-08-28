{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - All Data Combined ECHO Download Data Service",
    "_postman_id": "881c3ee8-e606-4a29-b39e-f6088f8563db",
    "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return a comma sepated vaule (CSV) file of the facilities found.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "c54d5793-fb12-46c2-9e6e-8f4b5d46a465",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/echo_rest_services.get_download?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
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
          "id": "70f472ad-dd71-4c2e-a20d-27a3254d48cd"
        }
      ]
    }
  ]
}