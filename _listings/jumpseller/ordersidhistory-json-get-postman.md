{
  "info": {
    "name": "Jumpseller Get Orders History",
    "_postman_id": "ded37dba-997d-4381-9ff3-462053e08fa1",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Orders",
      "item": [
        {
          "id": "06a78877-4f88-4d2a-89e6-74ef15ef3221",
          "name": "getOrdersHistory.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "orders/:id/history.json"
              ],
              "query": [
                {
                  "key": "No Name",
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
            "description": "Get Orders History"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b396c8e3-acec-4e9a-8586-0e9c26fcb92c"
            }
          ]
        }
      ]
    }
  ]
}