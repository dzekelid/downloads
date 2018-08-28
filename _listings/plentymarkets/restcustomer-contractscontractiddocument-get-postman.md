{
  "info": {
    "name": "Plentymarkets Starts download of contract document",
    "_postman_id": "ef8e0e42-5f69-4ad1-bdfc-b36739698ea6",
    "description": "Starts download of contract document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Starts",
      "item": [
        {
          "id": "8ac1bdf3-e521-4d91-9eec-73b83f4e69de",
          "name": "getRestCustomerContractsContractDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/customer_contracts/:contractId/document"
              ],
              "variable": [
                {
                  "id": "contractId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Starts download of contract document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97378d15-219b-47a5-b2bf-3d82c606ba3e"
            }
          ]
        }
      ]
    }
  ]
}