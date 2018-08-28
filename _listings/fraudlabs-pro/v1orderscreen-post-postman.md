{
  "info": {
    "name": "FraudLabs Pro V1OrderScreen_POST",
    "_postman_id": "6fd3f63e-196a-4edd-9f18-8379dcfe7242",
    "description": "Screen order for payment fraud.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Orders",
      "item": [
        {
          "id": "6c8ea3cf-99a4-41f5-b5e5-de87e9bb454b",
          "name": "V1OrderScreenPost",
          "request": {
            "url": "http://virtserver.swaggerhub.com/fraudlabspro/fraudlabspro/1.0/v1/order/screen?amount=%7B%7D&avs_result=%7B%7D&bill_addr=%7B%7D&bill_city=%7B%7D&bill_country=%7B%7D&bill_state=%7B%7D&bill_zip_code=%7B%7D&bin_no=%7B%7D&card_hash=%7B%7D&currency=%7B%7D&cvv_result=%7B%7D&department=%7B%7D&email=%7B%7D&email_domain=%7B%7D&email_hash=%7B%7D&first_name=%7B%7D&flp_checksum=%7B%7D&format=%7B%7D&ip=%7B%7D&key=%7B%7D&last_name=%7B%7D&password_hash=%7B%7D&payment_mode=%7B%7D&quantity=%7B%7D&ship_addr=%7B%7D&ship_city=%7B%7D&ship_country=%7B%7D&ship_state=%7B%7D&ship_zip_code=%7B%7D&username_hash=%7B%7D&user_order_id=%7B%7D&user_order_memo=%7B%7D&user_phone=%7B%7D",
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
            "description": "Screen order for payment fraud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfea5c24-0b89-4271-80f9-f28150963002"
            }
          ]
        }
      ]
    }
  ]
}