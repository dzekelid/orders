{
  "info": {
    "name": "Plentymarkets List order addresses",
    "_postman_id": "172c6b71-6dbc-467b-9870-cc72c38ae450",
    "description": "Lists order addresses. The ID of the order must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "b763660b-8e71-4eac-8d1a-1d818eb493f2",
          "name": "getRestAccountsContactsContactAddressesAddresstype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/addresses/:addressTypeId?"
              ],
              "variable": [
                {
                  "id": "addressTypeId?",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "contactId",
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
            "description": "Lists addresses of the contact. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b24b51a9-23fe-48be-ba57-1b8c05364ac8"
            }
          ]
        },
        {
          "id": "591d79c6-cf72-4431-b2ed-3409cccea46b",
          "name": "getRestOrdersOrderAddressesRelationtype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/:orderId/addresses/:relationTypeId?"
              ],
              "variable": [
                {
                  "id": "orderId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "relationTypeId?",
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
            "description": "Lists order addresses. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e78f1b6e-9853-45f6-a0c3-6dbd4e55e5c8"
            }
          ]
        }
      ]
    }
  ]
}