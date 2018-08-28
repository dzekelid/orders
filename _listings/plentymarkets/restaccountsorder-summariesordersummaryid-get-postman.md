{
  "info": {
    "name": "Plentymarkets Get an order summary by the order summary ID",
    "_postman_id": "3c9f1cb4-f019-4ada-b9af-eede0c1c1319",
    "description": "Gets an order summary. The ID of the order summary must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "5f2ebf0f-f469-44c8-8d66-66e79b41234b",
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
              "id": "35a3ee80-86e4-46dd-82a4-040c81a74c5c"
            }
          ]
        },
        {
          "id": "5169a96b-57e0-43bd-baa7-d0721242b25e",
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
              "id": "171b7d5c-d646-4901-8847-1c5d9b860f3a"
            }
          ]
        },
        {
          "id": "5446c75d-5cb4-4b84-bb03-996d937c7932",
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
              "id": "c135483a-ab3e-42a0-90ef-7b243a6b9615"
            }
          ]
        },
        {
          "id": "c87e3b31-9fe5-47dd-a08d-e9b05b6e8dd3",
          "name": "getRestAccountsOrderSummariesOrdersummary",
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
            "description": "Gets an order summary. The ID of the order summary must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fc97f41-e0c3-4db9-b94d-de9108c7ec20"
            }
          ]
        },
        {
          "id": "b81655b1-9101-476e-9d2f-21eccf5562e8",
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
              "id": "ffdf4d0b-c79a-4244-8788-ac8f8f86864a"
            }
          ]
        }
      ]
    }
  ]
}