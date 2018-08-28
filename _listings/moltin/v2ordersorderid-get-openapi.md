---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get a single order
  description: Get a single order.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/orders:
    get:
      summary: Get all orders
      description: Get all orders.
      operationId: V2OrdersGet
      x-api-path-slug: v2orders-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Orders
  /v2/orders/{orderID}:
    get:
      summary: Get a single order
      description: Get a single order.
      operationId: V2OrdersByOrderIDGet
      x-api-path-slug: v2ordersorderid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Single
      - Order
    put:
      summary: Update an order
      description: |-
        Transactions are created and updated automatically whenever you make a payment request. When a payment is successful, the transaction ID returned from the gateway will be attached to the transaction.

        It is possible for an order to have more than one transaction attached as each attempted payment will be created as a new transaction.
      operationId: V2OrdersByOrderIDPut
      x-api-path-slug: v2ordersorderid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Order
  /orders/{orderID}/items:
    get:
      summary: Get Order Items
      description: Get order items.
      operationId: OrdersItemsByOrderIDGet
      x-api-path-slug: ordersorderiditems-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Order
      - Items
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---