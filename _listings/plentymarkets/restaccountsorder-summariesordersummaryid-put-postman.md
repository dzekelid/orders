{
  "info": {
    "name": "Plentymarkets Update an order summary",
    "_postman_id": "bcd4dea7-a242-4494-a53e-c8febcd9b087",
    "description": "Updates an order summary. The ID of the order summary must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "622d0f5a-503b-4736-9f0f-ac45170f3ded",
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
              "id": "4e86c942-472d-41e1-a928-79bfc131b1f9"
            }
          ]
        },
        {
          "id": "b034efd4-fcb1-4ae6-ae45-8281de7bacdd",
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
              "id": "1168b35e-f9b4-48c3-b69f-6dccc79c7aca"
            }
          ]
        },
        {
          "id": "d49070bf-1138-4933-9498-451bdf3b7aad",
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
              "id": "e86d3806-93d3-42b3-8d18-79a845b862b5"
            }
          ]
        },
        {
          "id": "6bbee21b-9247-41f6-b561-fba15cb67042",
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
              "id": "f2d6171b-b20e-4521-8184-4b4d8e8ddcd9"
            }
          ]
        },
        {
          "id": "5d133b24-e95b-4dfc-a46a-0bf4257b430e",
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
              "id": "48f1f062-1a9c-4dab-b94c-665793b99b93"
            }
          ]
        },
        {
          "id": "666b8539-067f-4724-85de-fabab0ca4695",
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
              "id": "d9b2a1c3-7f50-4f67-8b41-93f243cc63cf"
            }
          ]
        }
      ]
    }
  ]
}