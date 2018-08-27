{
  "info": {
    "name": "Plentymarkets Starts download of signed contract document",
    "_postman_id": "f2b6870c-3ebd-43ee-a802-e9ce8f724ba6",
    "description": "Starts download of signed contract document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Starts",
      "item": [
        {
          "id": "e33f3e15-f67e-4431-999f-185060ad7595",
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
              "id": "f026e8dd-4693-4076-bd75-3edc94a7249d"
            }
          ]
        },
        {
          "id": "5505f7d0-4f25-4de3-b077-a5985a0d49e7",
          "name": "getRestCustomerContractsContractSignDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/customer_contracts/:contractId/sign/document"
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
            "description": "Starts download of signed contract document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c40efc0-e7aa-4d39-80e4-6050862f0e19"
            }
          ]
        }
      ]
    }
  ]
}