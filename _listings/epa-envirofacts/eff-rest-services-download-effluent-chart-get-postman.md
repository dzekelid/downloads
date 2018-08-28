{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Effluent Charting and Reporting Effluent Charts Download Service",
    "_postman_id": "5c124975-27b5-43f3-ab9a-242282eed9fe",
    "description": "Downloads tabular Discharge Monitoring Report (DMR) and compliance data for one NPDES permit as a CSV.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "86e6d5de-8205-414b-be82-2b9a41fcb454",
      "name": "downloads-tabular-discharge-monitoring-report-dmr-and-compliance-data-for-one-npdes-permit-as-a-csv-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/eff_rest_services.download_effluent_chart?No Name=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Downloads tabular Discharge Monitoring Report (DMR) and compliance data for one NPDES permit as a CSV."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "26ed588a-63c5-4689-9dc3-c5f2d160002a"
        }
      ]
    }
  ]
}