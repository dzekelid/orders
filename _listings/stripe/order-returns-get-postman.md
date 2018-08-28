{
  "info": {
    "name": "Stripe Get Order Returns",
    "_postman_id": "e853fe6e-2563-4097-8cf4-8b0fc85ff6b2",
    "description": "Returns a list of your order returns. The returns are returned sorted by creation date, with the most recently created return appearing first.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "order",
      "item": [
        {
          "id": "077b4e3b-534c-4912-976e-4cc9c33848f3",
          "name": "getOrderReturns",
          "request": {
            "url": "http://api.stripe.com/v1/order_returns?created=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&order=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your order returns"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2b5bfcc-f1f0-41ed-b4e4-7f9eae62bf9e"
            }
          ]
        }
      ]
    }
  ]
}