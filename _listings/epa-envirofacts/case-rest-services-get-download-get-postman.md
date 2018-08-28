{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Enforcement Case Search Enforcement Case Download Data Service",
    "_postman_id": "f4f171b1-07dd-4736-9df9-d8f372b7f682",
    "description": "Based on the QID obtained from a get_cases query, return a comma sepated vaule (CSV) file of the cases found.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "c7b6d5bc-6505-4719-92f5-0bafac7188c6",
      "name": "the-get-case-report-service-endpoint-returns-a-complex-object-of-civil-enforcement-case-details-base",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/case_rest_services.get_case_report?No Name=%7B%7D&output=%7B%7D&p_id=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The get_case_report service endpoint returns a complex object of civil enforcement case details based on the provided case id."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "98e679fc-114b-4739-9d8d-86dece39c30b"
        }
      ]
    },
    {
      "id": "5893878d-eea9-4e9d-a900-702ffc8e04e3",
      "name": "the-get-cases-service-end-point-searches-for-civil-enforcement-and-criminal-cases-based-on-the-provi",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/case_rest_services.get_cases?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The get_cases service end point searches for civil enforcement and criminal cases based on the provided selection criteria."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "179efb59-e0cf-4c0e-9753-415d20b33684"
        }
      ]
    },
    {
      "id": "c23d78a9-0cd6-4d4b-884d-e9ece282f54e",
      "name": "the-get-crcase-report-service-end-point-returns-a-complex-object-of-criminal-case-detials-based-on-t",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/case_rest_services.get_crcase_report?No Name=%7B%7D&output=%7B%7D&p_id=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The get_crcase_report service end point returns a complex object of criminal case detials based on the provided criminal case id."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d35d04c3-7caf-43a7-bd87-2d4fec6bb4e3"
        }
      ]
    },
    {
      "id": "5f9fa00b-a84b-454c-aae0-67d9fbd63003",
      "name": "based-on-the-qid-obtained-from-a-get-cases-query-return-a-comma-sepated-vaule-csv-file-of-the-cases-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/case_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_cases query, return a comma sepated vaule (CSV) file of the cases found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "1adbd3c3-b9eb-48a8-be43-1d812ab9b9ec"
        }
      ]
    }
  ]
}