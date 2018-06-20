{
  "info": {
    "name": "Stripe Get Orders",
    "_postman_id": "144f067f-8473-4e47-90ba-8f8fbf76769a",
    "description": "Retrieves the details of an existing order. Supply the unique order ID from either an order creation request or the order list, and Stripe will return the corresponding order information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "orders",
      "item": [
        {
          "id": "be1d3542-b055-4c63-8a15-09aa903aa218",
          "name": "getOrders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "orders/:id"
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
            "description": "Retrieves the details of an existing order"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9c68fcd-7d0a-472b-8046-3ced25cc6b2a"
            }
          ]
        }
      ]
    }
  ]
}