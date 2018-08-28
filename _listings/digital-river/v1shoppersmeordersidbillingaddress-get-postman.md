{
  "info": {
    "name": "Digital River Shopper API Get Shoppers Me Orders Billing Address",
    "_postman_id": "98a6cb3f-fe6f-4de5-a650-6a611285a98d",
    "description": "Get shoppers me orders billing address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shoppers",
      "item": [
        {
          "id": "b8bba49f-7d6a-41a4-bb98-726b71a55d96",
          "name": "getV1ShoppersMeCartsActiveBillingAddress",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/billing-address",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me carts active billing address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5509ad1c-16a7-4a45-bf58-4ec7ea6d32cd"
            }
          ]
        },
        {
          "id": "c3d323e2-6d64-4d51-aafb-7863e315653c",
          "name": "putV1ShoppersMeCartsActiveBillingAddress",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/billing-address",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Put shoppers me carts active billing address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ce40f09-2999-44e3-afea-4d01c897582d"
            }
          ]
        },
        {
          "id": "5390a1c7-6687-476f-995c-5e3ed130ae99",
          "name": "getV1ShoppersMeOrdersBillingAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/orders/:id/billing-address"
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
            "description": "Get shoppers me orders billing address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e098be5-a68b-4271-a816-132564b3adb8"
            }
          ]
        }
      ]
    }
  ]
}