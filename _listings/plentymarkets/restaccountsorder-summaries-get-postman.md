{
  "info": {
    "name": "Plentymarkets List order summaries",
    "_postman_id": "dedfb431-1334-44a8-89ce-39d056fb7c57",
    "description": "List order summaries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "39e51642-f75e-43b3-8ed6-386be08e91da",
          "name": "getRestAccountsOrderSummaries",
          "request": {
            "url": "http://example.com/rest/accounts/order_summaries",
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
            "description": "List order summaries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75bca948-2a29-420e-9e2f-2d910113ee50"
            }
          ]
        },
        {
          "id": "9ef84272-b073-44da-abd4-8836f3d9934f",
          "name": "getRestOrdersDocumentsAccountingSummary",
          "request": {
            "url": "http://example.com/rest/orders/documents/accounting_summary?createdAtFrom=%7B%7D&createdAtTo=%7B%7D&documentType=%7B%7D&itemsPerPage=%7B%7D&orderId=%7B%7D&page=%7B%7D",
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
            "description": "Lists document accounting summaries. A document accounting summary is saved along with each reversal document (for invoice and credit note). It contains accounting information about the order for this point in time. The summary is saved because an order can be updated after a reversal_document is generated. The information about the order before the update is needed for accounting."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "300db700-6fe6-41c4-a087-ef56ee4e2992"
            }
          ]
        }
      ]
    },
    {
      "name": "Order",
      "item": [
        {
          "id": "da3eec8e-c42f-4373-81a1-ec2b618a6a38",
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
              "id": "b6406e71-d753-425d-95e2-08ae0733badc"
            }
          ]
        },
        {
          "id": "4d5ab590-55b3-4d26-812d-96160e8eaf07",
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
              "id": "0bbbcb31-a7e3-4269-933b-45f1331dba4b"
            }
          ]
        },
        {
          "id": "819bacfb-fc97-40b7-9e08-a2dea3d8da34",
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
              "id": "ac11d916-28b9-4e0a-a913-889c96082d0d"
            }
          ]
        },
        {
          "id": "9d2b4612-d1c4-4a0b-b440-3750b340c551",
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
              "id": "e13ad4ea-5ce3-4290-bd48-4ab9d6c1ce14"
            }
          ]
        },
        {
          "id": "a3b1ebe6-42f5-4a2d-acae-20e2eafe2dd6",
          "name": "putRestAccountsOrderSummariesOrdersummary",
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
            "method": "PUT",
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
            "description": "Updates an order summary. The ID of the order summary must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54792396-a2cc-4b28-b854-2e82b9d3ca1d"
            }
          ]
        },
        {
          "id": "482b324f-34a2-43d9-8a2c-69cac1433cb3",
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
              "id": "645e4154-2707-41f1-a0a4-3d8bf43551a5"
            }
          ]
        }
      ]
    }
  ]
}