{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation and Recovery Act  Resource Conservation and Recovery Act (RCRA) Download Data Service",
    "_postman_id": "1b38facd-8d03-4c5c-8d98-842035c3c8db",
    "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return a comma sepated vaule (CSV) file of the facilities found.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "e7b6db89-63b1-4629-9708-f90544ec82a9",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
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
          "id": "95f87e4c-b39f-482c-a184-295acf881ed2"
        }
      ]
    }
  ]
}