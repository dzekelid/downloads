{
  "info": {
    "name": "Getty Images Search API Get Downloads",
    "_postman_id": "47be6c49-90dc-4d90-867b-4ba38fabd058",
    "description": "Returns information about a customer's downloaded assets..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Downloads",
      "item": [
        {
          "id": "83e7e920-1d45-4d13-9502-dc399a819491",
          "name": "getV3Downloads",
          "request": {
            "url": "http://api.gettyimages.com/v3/downloads?company_downloads=%7B%7D&date_from=%7B%7D&date_to=%7B%7D&page=%7B%7D&page_size=%7B%7D&product_type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Provide access token in the format of Bearer {token}",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a customer's downloaded assets.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "965a9b5f-07bf-4bd5-af7d-e22f05e9604e"
            }
          ]
        }
      ]
    }
  ]
}