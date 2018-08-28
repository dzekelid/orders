{
  "info": {
    "name": "Plentymarkets Create an order summary",
    "_postman_id": "456a2a59-7581-4217-9c19-625397596e85",
    "description": "Create an order summary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Order",
      "item": [
        {
          "id": "4803c5fa-5517-4dfe-8f86-01bf13497f1f",
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
              "id": "c34fc7a2-8ebe-48de-80aa-c01d3b1791ec"
            }
          ]
        }
      ]
    }
  ]
}