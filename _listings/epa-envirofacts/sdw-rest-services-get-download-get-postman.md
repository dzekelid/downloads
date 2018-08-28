{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Safe Drinking Water Act Safe Drinking Water Act (SDWA) Download Data Service",
    "_postman_id": "0d5733ea-e144-4172-b944-7fa11220ab67",
    "description": "Based on the QID obtained from a get_systems query, return a comma sepated vaule (CSV) file of the water systems found.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "2b2ae0a6-63d9-42ff-b57a-3dbf13c3e994",
      "name": "based-on-the-qid-obtained-from-a-get-systems-query-return-a-comma-sepated-vaule-csv-file-of-the-wate",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/sdw_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_systems query, return a comma sepated vaule (CSV) file of the water systems found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "19247ef5-55e7-46ee-8f2c-712254fb7499"
        }
      ]
    }
  ]
}