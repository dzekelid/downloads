{
  "info": {
    "name": "Plentymarkets Download the content of a document",
    "_postman_id": "c9eeb3d8-5b0c-42a3-a7f2-b68b3a6ce884",
    "description": "Downloads the content of a document. The ID of the document must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Download",
      "item": [
        {
          "id": "ac7938fa-0f6c-4b15-8f76-863e3f921cf3",
          "name": "getRestDocumentsDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/documents/:documentId"
              ],
              "variable": [
                {
                  "id": "documentId",
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
            "description": "Downloads the content of a document. The ID of the document must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cba58b8e-d180-4111-b4e3-9100bb0e9386"
            }
          ]
        }
      ]
    }
  ]
}