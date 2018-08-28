{
  "info": {
    "name": "Plentymarkets Delete an order summary",
    "_postman_id": "b530f1fc-83c5-4a18-99a8-f72fa98b3f0f",
    "description": "Deletes an order summary. The ID of the order summary must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "df997a5e-7c85-4fd6-a252-d21f88b09f9a",
          "name": "postRestAccountsOrderSummaries",
          "request": {
            "url": "http://example.com/rest/accounts/order_summaries",
            "method": "POST",
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
            "description": "Create an order summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d14b25de-a96f-4ffa-9dae-36d7e9c23160"
            }
          ]
        },
        {
          "id": "8bb95c12-ce15-4ea9-ae27-cd150b9b3f5e",
          "name": "getRestAccountsOrderSummariesContactsContact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/order_summaries/contacts/:contactId"
              ],
              "variable": [
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
            "description": "Gets an order summary. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a729f466-bc0f-4424-97fe-648e51b09373"
            }
          ]
        },
        {
          "id": "8ca345d1-e78f-4ed4-985e-f4b4e0c614f4",
          "name": "getRestAccountsOrderSummariesOrdersAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/order_summaries/orders/:addressId"
              ],
              "variable": [
                {
                  "id": "addressId",
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
            "description": "Gets an order summary. The ID of the address must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eab8efd4-e53d-4b85-ad20-a271cffffdf9"
            }
          ]
        },
        {
          "id": "a6dccc6d-e7fe-4319-9806-856cf8da1979",
          "name": "deleteRestAccountsOrderSummariesOrdersummary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/order_summaries/:orderSummaryId"
              ],
              "variable": [
                {
                  "id": "orderSummaryId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Deletes an order summary. The ID of the order summary must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5aae100-feb2-47c6-a031-e882b7429e80"
            }
          ]
        }
      ]
    }
  ]
}