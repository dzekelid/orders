{
  "info": {
    "name": "Steem get_order_book",
    "_postman_id": "e5ef2b3f-6af4-4368-8b1c-21492e818212",
    "description": "get_order_book",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "9d5fe506-f88b-4f32-90de-0be20f0c0b48",
          "name": "get-order-book",
          "request": {
            "url": "http://api.steemjs.com/get_order_book?limit=%7B%7D",
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
            "description": "get_order_book"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3468a00-54d8-4308-9dd7-df1c464f8dec"
            }
          ]
        }
      ]
    }
  ]
}