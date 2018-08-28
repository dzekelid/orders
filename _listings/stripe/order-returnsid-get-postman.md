{
  "info": {
    "name": "Stripe Get Order Returns",
    "_postman_id": "1639ad1d-3d9d-4e5c-a975-181c742b24aa",
    "description": "Retrieves the details of an existing order return. Supply the unique order ID from either an order return creation request or the order return list, and Stripe will return the corresponding order information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "order",
      "item": [
        {
          "id": "129004c6-a47a-4e8a-9a21-cc1637003fe5",
          "name": "getOrderReturns",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "order_returns/:id"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details of an existing order return"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab241132-1c6f-49d3-8643-28b91efb1ae9"
            }
          ]
        }
      ]
    }
  ]
}