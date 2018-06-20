{
  "info": {
    "name": "Google Content API for Shopping API Get Orders",
    "_postman_id": "c5cdb9f1-0416-4f40-9874-d078ffe89965",
    "description": "Lists the orders in your Merchant Center account. This method can only be called for non-multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "orders",
      "item": [
        {
          "id": "e24dcec8-fb45-4f30-8a40-2e69b57c714a",
          "name": "content.orders.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/orders"
              ],
              "query": [
                {
                  "key": "acknowledged",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "placedDateEnd",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "placedDateStart",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "statuses",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "merchantId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the orders in your Merchant Center account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "993a3e18-df01-4437-aa7d-735824cbc504"
            }
          ]
        }
      ]
    }
  ]
}