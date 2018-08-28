swagger: "2.0"
x-collection-name: Etsy
x-complete: 1
info:
  title: Etsy
  description: bring-etsys-handmade-marketplace-and-community-into-your-apps-
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/{order_id}:
    get:
      summary: Get Orders Order
      description: Retrieves a Order by id.
      operationId: getOrdersOrder
      x-api-path-slug: ordersorder-id-get
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
  /orders/{order_id}/receipts:
    get:
      summary: Get Orders Order Receipts
      description: Retrieves a set of Receipt objects associated to a Order.
      operationId: getOrdersOrderReceipts
      x-api-path-slug: ordersorder-idreceipts-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Receipts
  /users/{user_id}/orders:
    get:
      summary: Get Users User Orders
      description: Retrieves a set of Order objects associated to a User.
      operationId: getUsersUserOrders
      x-api-path-slug: usersuser-idorders-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Orders